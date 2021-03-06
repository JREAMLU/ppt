# 熔断与限流

---

## About Me

-   作者: LU
-   时长: 大约40分钟

---

## 熔断

---

## 什么是熔断

---

## 为什么要熔断

-   过载保护机制 |
-   客户端请求量大 |
-   并且服务端出现大量失败或超时 |
-   防止过多错误导致服务器雪崩 |
-   保险丝 |
-   一般在客户端进行保护 |

---

## 熔断实现原理

---

## 熔断的三种状态

<br/>
-   闭合(Closed) |
-   半断开状态(HalfOpen) |
-   断开状态(Open) |

---

## 熔断的请求统计

<br/>
-   请求数 |
-   请求成功数 |
-   请求失败数 |
-   连续成功数 |
-   连续失败数 |

---

## 熔断的过程

-   正常访问 |
-   服务端出现一定量的失败或超时 |
-   命中条件 |
-   进入断开状态 |
-   等待时间 |
-   进入半断开状态 |
-   允许一定的流量进入 |
-   没毛病则进入闭合 |
-   有毛病则继续进入断开 |

---

## 阅读源码

[https://github.com/sony/gobreaker](https://github.com/JREAMLU/gobreaker)

---

## 熔断实际演示

---

## 熔断(完)

---

# 限流

---

## 什么是限流

---

## 为什么要限流

-   大流量涌入 |
-   突刺 |
-   抢购 |
-   防止过大流量导致服务器雪崩 |
-   客户端服务端都可以限流 |
-   不同的服务设置各自流量 |

---

## 限流的方式

-   漏桶算法 |
-   令牌桶算法 |

---

## 漏桶算法原理

---?image=assets/image/bucket.png&size=auto 60%&color=white

---

## 令牌桶算法原理

---?image=assets/image/token-bucket.png&size=auto 60%&color=white

---

## 阅读源码

[https://github.com/juju/ratelimit](https://github.com/JREAMLU/ratelimit)

---

## 限流实际演示

---

## 限流与熔断的区别

<br>
@fa[check] 熔断具有状态性, 试探性

@fa[check] 限流则更直接

---

## 全剧(终)

---

## Questions?

---

### Thank You

@fa[github gp-contact](JREAMLU)
