<style>
.green {
    color: green;
    font-weight:700;
    font-size: 40px;
}
</style>

<div class="green">
*مرسال*
</div>

# *mersal*  *مرسال*

##### Instant messaging server, easy to use as a server or as a library

### install :
```go get -u github.com/bashery/im```

### how to use ?

create a websocket on browser and send message as json :

to subscribe in a topic (channel) send :
```json
{
   "event":"subscribe",
   "channel":"my-channel-id"
}
```
```event``` must be : ```subscribe```, ```unsubscribe```, ```message```,

Later we will add events:  ```reseive```, and```seen```,
We will also work to achieve quality service ```qos``` .

to send message to channel/topic:
```json
{
   "event" : "message",
   "channel" : "my-channel-123",
   "data" : "hi frends"
}
```
then all client subscribe with "my-channel-123" will be receive "hi frinds" message.

### How do I create a private connection? between two clients?
Just create a channel and share it between two clients only, this is how you create a private connection

### Project status
- [x] websocket
- [x] Pubsub 
- [ ] cache message
- [ ] Unit testing
- [ ] Qos
- [ ] ssl

### Not goal or maybe later
- [ ] End-to-end encryption


