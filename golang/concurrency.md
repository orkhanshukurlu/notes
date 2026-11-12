1. Concurrency fundamentals
- Concurrency vs Parallelism
- Processes vs Threads
- Concurrency vs Multithreading
- Go concurrency model
- Goroutines
- Go runtime scheduler
- G, M, P model (Goroutine, Machine, Processor)
- Cooperative and preemptive scheduling
- GOMAXPROCS

2. Goroutines
- Creating goroutines (go keyword)
- Goroutine lifecycle
- Goroutine scheduling
- Goroutine stacks
- Goroutine leaks
- Anonymous goroutines
- Goroutine synchronization
- Managing goroutine lifecycles

3. Channels
- What are channels?
- Unbuffered channels
- Buffered channels
- Sending and receiving data
- Closing channels
- Receiving from closed channels
- Nil channels
- Directional channels (chan<-, <-chan)
- Channel blocking
- Channel deadlocks
- Channel ownership patterns

4. Synchronization primitives (sync package)
- sync.WaitGroup
- sync.Mutex
- sync.RWMutex
- sync.Once
- sync.Cond
- sync.Map
- sync.Pool
- sync/atomic
- Atomic operations
- Compare-and-swap (CAS)

5. Select statement
- What is select?
- Multiple channel operations
- Default case
- Timeout handling
- Non-blocking channel operations
- Handling multiple channels
- Select with context cancellation

6. Context and cancellation
- What is context.Context?
- context.Background()
- context.TODO()
- context.WithCancel()
- context.WithTimeout()
- context.WithDeadline()
- context.WithValue()
- Parent-child context relationships
- Graceful shutdown
- Cancellation propagation

7. Concurrency patterns
- Worker Pool Pattern
- Fan-out / Fan-in
- Pipeline Pattern
- Generator Pattern
- Producer-Consumer Pattern
- Semaphore Pattern
- Bounded Concurrency
- Rate Limiting
- Request Throttling
- Singleflight Pattern
- Or-Done Channel Pattern
- Graceful Shutdown Pattern

8. Problems and pitfalls
- Race Conditions
- Deadlocks
- Data Races
- Goroutine Leaks
- Resource Contention
- Mutex Contention
- Starvation
- Livelocks
- False Sharing
- Concurrent Map Access
- Double Close of Channels
- Sending to Closed Channels

9. Memory model and advanced concepts
- Go Memory Model
- Happens-Before Relationship
- Synchronization Ordering
- Atomicity
- Memory Visibility
- Sequential Consistency
- Lock-Free Programming
- Compare-and-Swap (CAS)
- Cache Coherence
- CPU Memory Barriers

10. Runtime and performance
- Go Runtime Scheduler
- G-M-P Scheduler Model
- Work Stealing
- Goroutine Preemption
- Stack Growth
- Thread Management
- GOMAXPROCS
- CPU-bound vs I/O-bound workloads
- runtime.NumGoroutine()
- runtime/trace
- net/http/pprof
- Benchmarking concurrent code
- Profiling and performance optimization

11. Useful standard library packages
- sync           - Synchronization primitives
- sync/atomic    - Atomic operations
- context        - Cancellation and deadlines
- runtime        - Runtime and scheduler
- time           - Timers and tickers
- net/http       - Concurrent HTTP operations
- runtime/trace  - Execution tracing
- net/http/pprof - Performance profiling