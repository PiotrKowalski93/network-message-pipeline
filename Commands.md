### Producer

```bash
# Windows
cmake -S . -B build/producer -DBUILD_PRODUCER=ON 
cmake --build build/producer

.\build\producer\producer\Debug\producer.exe

# Linux
cmake -S . -B build/producer -DBUILD_PRODUCER=ON 
cmake --build build/producer -j$(nproc)
```

### Consumer

```bash
# Windows
cmake -S . -B build/consumer -DBUILD_CONSUMER=ON 
cmake --build build/consumer

.\build\consumer\consumer\Debug\consumer.exe

# Linux
cmake -S . -B build/producer -DBUILD_CONSUMER=ON 
cmake --build build/producer -j$(nproc)
```