# Package [sync](https://pkg.go.dev/sync)
Package sync provides basic synchronization primitives such as mutual exclusion locks.  
Other than the Once and WaitGroup types, most are intended for use by low-level library routines.  
Higher-level synchronization is better done via channels and communication.  

Values containing the types defined in this package should not be copied.  

Useful Types:  
```go
WaitGroup
- (wg *WaitGroup) Add(delta int)
- (wg *WaitGroup) Done()
- (wg *WaitGroup) Wait()

Mutex // Mutual Exclusion
- (m *Mutex) Lock()
- (m *Mutex) Unlock()
```