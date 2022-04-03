## 1 - emmc compiler libwebp

```
emcc -O3 -s WASM=1 -s EXPORTED_RUNTIME_METHODS='["cwrap"]' /
    -I libwebp -s ERROR_ON_UNDEFINED_SYMBOLS=0 /
    webp.c /
    libwebp/src/{dec,dsp,demux,enc,mux,utils}/*.c
```