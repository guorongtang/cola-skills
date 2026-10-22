# Cola Skills

ColaSkill 官方技能仓库。每个目录是一个可独立安装的 Agent Skill，目录内的 `SKILL.md` 是技能入口。

## 技能列表

| 技能 | 目录 | 发布时间（北京时间） | 说明 |
| --- | --- | --- | --- |
| Cola 美团领券 | [`cola-meituan-coupon`](./cola-meituan-coupon) | 2026-10-20 11:51 | 报一次手机号验证码，之后每天自动把外卖、买菜、闪购券领进美团账户 |
| 中国移动 AI 豆兑换本机话费 | [`cmcc-points-redeem`](./cmcc-points-redeem) | 2026-10-16 15:33 | 中国移动积分商城 AI 豆零现金兑换本机话费，含短信验证交接与到账核对 |
| 京东价格保护申请与退款核对 | [`jd-price-protection`](./jd-price-protection) | 2026-10-16 14:10 | 查降价、申请价保、追踪价保退款，支持中断恢复 |
| 京东京豆领取与签到 | [`jd-bean-claim`](./jd-bean-claim) | 2026-10-15 14:02 | 购物返豆补领、每日签到与到账核对 |
| 联通积分兑换流量、语音与影音权益 | [`cucc-points-redeem`](./cucc-points-redeem) | 2026-10-20 17:54 | 联通积分盘点与兑换，Agent 准备结算并由本人完成验证 |
| 淘宝天猫算账助手 | [`promo-shopping-assistant`](./promo-shopping-assistant) | 2026-10-21 18:39 | 读取购物车，核对立减、折扣、满减券、红包和金币，给出更省钱的买法 |
| 提 Issue 指南 | [`report-issues-to-cola`](./report-issues-to-cola) | — | 让 Cola 按统一规范收集上下文并向 `cola-public-feedback` 提交 Issue |

## 使用方式

在 Cola 对话中直接说：

```text
学习 https://github.com/marswaveai/cola-skills/tree/main/cola-meituan-coupon 下的内容
```

把链接换成上表中的任意目录即可。

也可以手动安装：将技能目录复制到 `~/.cola/skills/`（Windows 为 `%USERPROFILE%\.cola\skills\`），重启会话后生效。

## 目录结构

```text
cola-skills/
├── cola-meituan-coupon/        # SKILL.md + scripts/ + README
├── cmcc-points-redeem/         # SKILL.md + LICENSE
├── jd-price-protection/        # SKILL.md + LICENSE
├── jd-bean-claim/              # SKILL.md + scripts/ + references/ + tests/
├── cucc-points-redeem/         # SKILL.md + agents/ + references/ + scripts/ + tests/
├── promo-shopping-assistant/   # SKILL.md + scripts/ + references/ + fixtures/ + tests/
└── report-issues-to-cola/      # 提 Issue 规范与流程
```

## 来源与许可

| 目录 | 来源 | 许可 |
| --- | --- | --- |
| `cola-meituan-coupon` | Cola 官方基于美团开放平台官方技能 `meituan-coupon` v1.0.10 定制 | 上游未附许可证 |
| `cmcc-points-redeem` | <https://github.com/huntingrin/cmcc-points-redeem> | MIT |
| `jd-price-protection` | <https://github.com/huntingrin/jd-price-protection> | MIT |
| `jd-bean-claim` | <https://github.com/huntingrin/jd-bean-claim> | MIT |
| `cucc-points-redeem` | <https://github.com/huntingrin/cucc-points-redeem> | 未声明 |
| `promo-shopping-assistant` | <https://github.com/huntingrin/promo-shopping-assistant> | 未声明 |

各技能涉及的账号、验证码与登录态均由使用者在本地自行完成，仓库内不包含任何凭证。
