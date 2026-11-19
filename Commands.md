```bash
# Windows
cmake -S . -B Build/producer -DBUILD_PRODUCER=ON 
cmake --build Build/producer

.\build\producer\producer\Debug\producer.exe

# Linux
cmake -S . -B Build/producer -DBUILD_PRODUCER=ON 
cmake --build Build/producer -j$(nproc)
```