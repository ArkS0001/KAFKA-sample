# KAFKA-sample

```
📤 Producer: Sending -> Message 1
📤 Producer: Sending -> Message 2
📤 Producer: Sending -> Message 3
🔀 Broker: Routed -> Message 1 to Consumer-1
🔀 Broker: Routed -> Message 2 to Consumer-2
✅ Consumer-1: Received -> Message 1
🔀 Broker: Routed -> Message 3 to Consumer-3
✅ Consumer-2: Received -> Message 2
✅ Consumer-3: Received -> Message 3
📤 Producer: Sending -> Message 4
🔀 Broker: Routed -> Message 4 to Consumer-1
📤 Producer: Sending -> Message 5
🔀 Broker: Routed -> Message 5 to Consumer-2
✅ Consumer-1: Received -> Message 4
✅ Consumer-2: Received -> Message 5
📤 Producer: Sending -> Message 6
🔀 Broker: Routed -> Message 6 to Consumer-3✅ Consumer-3: Received -> Message 6

📤 Producer: Sending -> Message 7
🔀 Broker: Routed -> Message 7 to Consumer-1
✅ Consumer-1: Received -> Message 7
📤 Producer: Sending -> Message 8
🔀 Broker: Routed -> Message 8 to Consumer-2✅ Consumer-2: Received -> Message 8

📤 Producer: Sending -> Message 9
🔀 Broker: Routed -> Message 9 to Consumer-3
✅ Consumer-3: Received -> Message 9
📤 Producer: Sending -> Message 10
🔀 Broker: Routed -> Message 10 to Consumer-1✅ Consumer-1: Received -> Message 10

🔴 Consumer-2: Stopping.
🔴 Consumer-3: Stopping.
🔴 Consumer-1: Stopping.
🚀 Kafka-like pipeline with Round-Robin broker complete!
```
