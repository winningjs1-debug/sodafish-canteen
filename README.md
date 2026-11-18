# SodaFish 小食堂 · 复古车票风点单台

GitHub Pages 版。`index.html` / `notes.html` / `admin.html` 是轻量包装页（沙箱 iframe），
真正的页面是 `app-canteen.html` / `app-notes.html` / `app-admin.html`。

- `index.html` — 菜单点单台（实时票数、下单出票、取餐码查询、主厨赞赏）
- `notes.html` — 点菜便签（智能总结、评分、讨论区）
- `admin.html` — 店主后台（页脚「店主入口」，口令进入）

> 为什么要包一层 iframe：云端数据库只对受信任来源开放跨域预检，
> 沙箱 iframe 以 `Origin: null` 发请求可正常通过，数据实时互通。
