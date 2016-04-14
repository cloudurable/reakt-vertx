# Reakt Vertx
Added Promises and simplified streaming to Vert.x

```java
        final Promise<Employee> promise = Promises.<Employee>promise();
        promise.thenExpect(this::handleResult).catchError(this::handleError);
        /** Convert the Reakt promise to a Vert.x asyncResultHandler */
        final Handler<AsyncResult<Employee>> asyncResultHandler = ReaktVertx.convertPromise(promise);
```


You can also use replay promises, all promises, any promises, and other
features of Reakt to simplify async, reactive Vertx/Java development.

Reakt gets used by [QBit](http://advantageous.github.io/qbit/), and Conekt.

#### Related projects
* [QBit Reactive Microservices](http://advantageous.github.io/qbit/)
* [Reakt Reactive Java](http://advantageous.github.io/reakt)
* [Reakt Guava Bridge](http://advantageous.github.io/reakt-guava/)
* [QBit Extensions](https://github.com/advantageous/qbit-extensions)
* [Czar Maker Consul](http://advantageous.github.io/czar-maker-consul/)
* [Czar Maker](http://advantageous.github.io/czar-maker/)
* [Reactive Microservices](http://www.mammatustech.com/reactive-microservices)
