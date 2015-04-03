# Real-Time Private Messaging Demo Using STOMP Over WebSockets on Spring Boot

This project demonstrates the use of [STOMP](https://stomp.github.io/) over WebSockets on Spring Boot in conjunction with [Apache ActiveMQ](http://activemq.apache.org) and [Apache Camel](http://camel.apache.org) to send data to clients in real-time. For a more detailed explanation, visit the blog page at [http://yalingunayer.com/blog/realtime-data-delivery-on-spring-boot-using-activemq-and-stomp-over-websockets-part-2](http://yalingunayer.com/blog/realtime-data-delivery-on-spring-boot-using-activemq-and-stomp-over-websockets-part-2)

## Prerequisites

- [Gradle](https://gradle.org/)
- [Apache ActiveMQ](http://activemq.apache.org)

## Running

Install and run your ActiveMQ instance. If the address your ActiveMQ is running on is not ```tcp://localhost:61616``` change the configuration at ```src/main/java/messaging/config/CamelConfig.java```

Once ActiveMQ starts running, run the application with the command ```gradle bootRun```

Visit ```http://localhost:8080``` to access the UI.

Login with one of the following users:

| Username | Password |
| ------ | ------ |
| user1 | pass1 |
| user2 | pass2 |
| user3 | pass3 |

Make sure to login with different users on different browser sessions (multiple browsers or browser tabs) to demonstrate both user-specific and broadcast message delivery in real-time.

## License

[Public Domain](http://choosealicense.com/licenses/unlicense/), or in other words, do whatever you want with it, but I provide no warranties of any kind so I can't be held responsible for any damages it may cause.