# Stupid Fancy Words
*Explaining the fancy words in software industry*

## `Uncategorized`

- **Fire/Call/Trigger/Invoke :** you will see these words a lot and everywhere, it just means execute/run a function.

- **Compile :** Compiler transforms code written in a high-level programming language into the machine code, at once (all code in a file), before program runs.

- **Interpreter :** Converts each high-level program statement (instruction/code block... whatever), one by one, into the machine code, during program run.

- **Transpile :** Convert the syntax of one programming language to another. That's it.

- **High-level programming :** its simply a programming language that is human readable and easy to write, read and maintain. Examples of high level languages are C, C++, Java, Python, etc.

- **Low-level programming :** its programming language that is machine friendly, It is tough to understand and complex to maintain, It is not commonly used now-a-days in programming. so rest 😅

- **Unit Test :** its nothing but testing your code. for example testing functions if they are working and returning values you expect.

- **Stream / Data stream... :** simply means data being sent somewhere (e.g, to a server) over time. A stream can be thought of as items on a conveyor belt being processed one at a time rather than in large batches.

- **Buffer :** A buffer contains data that is stored for a short amount of time, typically in the computer's memory (RAM). The purpose of a buffer is to hold data right before it is used. For example, when you download an audio or video file from the Internet, it may load the first 20% of it into a buffer and then begin to play.

- **Pub/Sub :** Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service (e.g: user and user cart) communication. for example service A, B, C subscribe to a topic (like a youtube channel, the channel is the topic) and when data is published to that topic the subscribers will get that data immediately. think of it like a youtube channel when the channel publish a new video the subscribers will be notified. 

- **Server :** its just a machine, a computer like yours that have an OS, a RAM a CPU... that stores your source code (files) and runs it.

- **Client :** client in software has many meanings, but in general it means the consumer, it can be the browser (wich is you) it can be any thing that consume or use a software.

- **Web Server :** It can be a Software or Hardware (a computer/machine) that runs websites, it just takes your button click and deliver it to the server (the code you write) and get the response back to you (who clicked that button)

- **API :** its nothing but a web server (code you write e.g: using Nodejs, Python...) that respond to user requests (e.g: creating an account) with Fail or Success messages.

- **Vanilla / Pure :** its just refers to the pure/parent programming language.

- **Anonymous :** its just a function that doesn't have a name, e.g: ``` const foo = function() { ... } ```, python example ``` bar = lambda x, y : ... ```

----

## `Computing`

- **Computing :** Computing is any activity that uses computers to manage, process, and communicate information. It includes development of both hardware and software.

- **Cluster :** A cluster, refers to a group of machines that work together that perform a similar function. a computer cluster is controlled by a single software program that manages all the computers (also called "nodes") within the cluster. The nodes work together to complete a single task. This process is called "parallel computing" since the nodes perform operations in tandem. 
  Computer clusters can range from two machines to hundreds of connected computers. Small clusters are often used to improve the performance of web and online gaming services by handling multiple incoming requests in parallel.


## `js`

- **Closures :** Its just a function that returns a function.

- **Single-threaded :** means the execution of single code instruction at a time.

- **Hoisting :** Its just a memory space that the javascript engine sets up before executing your code. it sets up a memory space for your variables and functions, thats what explains when you call your function and then actually create it works, its already there in memory and javascript recognize it when it sees it, and for variables they are set to "undefined".

- **Event Loop :** it will take some more words to explain, here is a [good article for you to read](https://medium.com/front-end-weekly/javascript-event-loop-explained-4cd26af121d4)

- **Execution Context :** every js code you write (functions) javascript engine creates an execution context for it, Its a wrapper to help manage the code that is running. it contains your runnning code (e.g: functions) and also things beyond what you wrote, like the "this object" and the global object and all that stuff that the javascript engine create for you.

- **Execution Stack :** Its just a stack 📚 of execution contexts, and which ever one at the top its the one that is currently running.

- **Callback :** its just a function that is used as a parameter in some function.

- **Scope :** is where a variable available in your code. means where its defined and where you can use it.
e.g:
```js
function greet(){
  let a = "hello";
  
  return a;
}

console.log(greet())
console.log(a);
// if you run this code, you will get an error, cause "a" is not defined.
```

- **Synchronous :**

- **Asynchronous :**

- **Primitve Types :**

- **Functional Programming :**

- **Immediately Invoked Functions (IIFEs) :**

## `Databases`

- **ACID-compliant :** Stands for "Atomicity, Consistency, Isolation, Durability." The ACID acronym defines four characteristics a database must have to ensure data integrity  

  0. **Transaction :** A transaction is a mechanism that allows you to mark a group of operations ***(sql queries)*** and execute them in such a way that either they all execute (commit), or the system state will be as if they have not started to execute at all (rollback).
  e.g:
  ```sql
  -- BEGIN TRANSACTION
  -- transfer $100 for example from one account to another
    UPDATE users SET balance = balance + 100 WHERE user_id = 5;
    UPDATE users SET balance = balance - 100 WHERE user_id = 2;
    -- SELECT * FROM users WHERE user_id = 2;
    -- ...
  -- END TRANSACTION
  ``` 
  1. **Atomicity :** Atomicity guarantees each transaction is an "all-or-nothing" event. In other words, it succeeds or fails completely. Atomic operations prevent data corruption by disallowing partial transactions. If an operation cannot be completed, it is "rolled back" to the previous state, as if it never happened.

  2. **Consistency :** Consistency means that you guarantee that your data will be consistent; none of the constraints you have on related data will ever be violated.

  3. **Isolation :** Isolation means that one transaction cannot read data from another transaction that is not yet completed. If two transactions are executing concurrently, each one will see the world as if they were executing sequentially, and if one needs to read data that is written by another, it will have to wait until the other is finished.

  4. **Durability :** means that once a transaction is complete, it is guaranteed that all of the changes have been recorded to a durable medium (such as a hard disk), and the fact that the transaction has been completed is likewise recorded.


## `Front End`

- **Lazy loading :** is a technique that delays loading resources (images, videos, ...) until they are needed. A common example is a webpage that defers loading images until the user scrolls to their location within the page.
  Lazy loading videos is also popular on the web. It is especially effective since video files are typically the largest resources loaded within a webpage. Instead of sending the entire video to a client's device, the web server only sends small portions of the video while the user is watching it. Popular video sharing websites like YouTube and Vimeo use lazy loading.


## TODO
- [ ] Finish the JS fancy words  
- [ ] Add more fancy words
- [ ] Add examples

