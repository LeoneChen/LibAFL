# Pre 0.9 -> 0.9
- [Migrating from LibAFL <0.9 to 0.9](https://aflplus.plus/libafl-book/design/migration-0.9.html)

# 0.14.0 -> 0.14.1
- Removed `with_observers` from `Executor` trait.
- `MmapShMemProvider::new_shmem_persistent` has been removed in favour of `MmapShMem::persist`. You probably want to do something like this: `let shmem = MmapShMemProvider::new()?.new_shmem(size)?.persist()?;`
