# Algorithms

Since version 2 mining [algorithm](#algorithm-names) should specified for each pool separately (`algo` option), earlier versions was use one global `algo` option and per pool `variant/powVariant` option (this option was removed in v2). If your pool support [mining algorithm negotiation](https://github.com/xmrig/xmrig-proxy/issues/168) you may not specify this option at all.
 
#### Example
```json
{
  "pools": [
    {
      "url": "...",
      "algo": "cn/r",
      ...
    }
 ],
 ...
}
```

#### Pools with mining algorithm negotiation support.

 * [www.hashvault.pro](https://www.hashvault.pro/)
 * [moneroocean.stream](https://moneroocean.stream)
 
 ## Algorithm names

| Name | Memory | Version | Notes |
|------|--------|---------|-------|
| `rx/test` | 2 MB | 2.0.0+ | RandomX (reference configuration). |
| `rx/0` | 2 MB | 2.0.0+ | RandomX (reference configuration), reserved for future use. |
| `rx/wow` | 1 MB | 2.0.0+ | RandomWOW. |
| `rx/loki` | 2 MB | 2.0.0+ | RandomXL. |
| `cn/conceal` | 2 MB | 1.9.5+ | CryptoNight variant 1 (modified). |
| `argon2/chukwa` | 512 KB | 1.9.5+ | Argon2id (Chukwa). |
| `argon2/wrkz` | 256 KB | 1.9.5+ | Argon2id (WRKZ). |
| `cn-extremelite/upx2` | 128 KB | <1.9.5 | CryptoNight-Extremelite variant UPX2 with reversed shuffle. |
| `cn/fast` | 2 MB | <1.9.5+ | CryptoNight variant 1 with half iterations. |
| `cn/rwz` | 2 MB | <1.9.5+ | CryptoNight variant 2 with 3/4 iterations and reversed shuffle operation. |
| `cn/zls` | 2 MB | <1.9.5+ | CryptoNight variant 2 with 3/4 iterations. |
| `cn/double` | 2 MB | <1.9.5+ | CryptoNight variant 2 with double iterations. |
| `cn/r` | 2 MB | <1.9.5+ | CryptoNightR (Monero's variant 4). |
| `cn/wow` | 2 MB | <1.9.5+ | CryptoNightR (Wownero). |
| `cn-pico` | 256 KB | <1.9.5+ | CryptoNight-Pico. (Turtle) |
| `cn/half` | 2 MB | <1.9.5+ | CryptoNight variant 2 with half iterations. |
| `cn/2` | 2 MB | <1.9.5+ | CryptoNight variant 2. |
| `cn/xao` | 2 MB | <1.9.5+ | CryptoNight variant 0 (modified). |
| `cn/rto` | 2 MB | <1.9.5+ | CryptoNight variant 1 (modified). |
| `cn-heavy/tube` | 4 MB | <1.9.5+ | CryptoNight-Heavy (modified). |
| `cn-heavy/xhv` | 4 MB | <1.9.5+ | CryptoNight-Heavy (modified). |
| `cn-heavy/0` | 4 MB | <1.9.5+ | CryptoNight-Heavy. |
| `cn/1` | 2 MB | <1.9.5+ | CryptoNight variant 1. |
| `cn-lite/1` | 1 MB | <1.9.5+ | CryptoNight-Lite variant 1. |
| `cn-lite/0` | 1 MB | <1.9.5+ | CryptoNight-Lite variant 0. |
| `cn/0` | 2 MB | <1.9.5+ | CryptoNight (original). |
