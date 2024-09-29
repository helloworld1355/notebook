### 连接kafka

从2.5版本开始，每一个都拓展了`KafkaResourceFactory`。允许在运行时通过添加一个`Supplier<String>`使用`setBootstrapServersSupplier(() -> …)`设置配置选项，来修改他们的引导服务。消费者和生产者通常寿命较长。为了关闭存在的生产者，在`DefaultKafkaProducerFactory`使用`reset()`。关闭存在的消费者，使用`KafkaListenerEndpointRegistry`的`start()`
