# TOPIC 熔断与限流

---

## About Me

-   Author - LU

---

## 熔断

[https://github.com/sony/gobreaker](https://github.com/sony/gobreaker)

---

## 什么是熔断

-   过载保护 |
-   客户端请求量大 |
-   服务端出现大量错误 |
-   保险丝 |

---

## 熔断实现原理

---

## 熔断的三种状态

<br/>
-   @fa[check] 闭合(Closed) |
-   @fa[check] 半断开状态(HalfOpen) |
-   @fa[check] 断开状态(Open) |

---

## 熔断的请求统计

<br/>
-   @fa[check] 请求数 |
-   @fa[check] 请求成功数 |
-   @fa[check] 请求失败数 |
-   @fa[check] 连续成功数 |
-   @fa[check] 连续失败数 |

---

## 熔断的过程

-   正常访问 |
-   服务端出现错误 |
-   命中条件 |
-   进入断开状态 |
-   等待时间 |
-   进入半断开状态 |
-   允许一定的流量进入 |
-   没毛病则进入闭合 |
-   有毛病则继续进入断开 |

---

## 阅读源码

---

## 熔断实际演示

---

## 熔断(完)

---

# 限流

---

## Questions?

---

### END

<br>

@fa[github gp-contact](JREAMLU)

## Thank You
