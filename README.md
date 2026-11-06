# 寸金 · CunJin

项目及 Git 仓库名称：`cunjin-site`。

独立的寸金产品介绍网站。黑金主题、中英文介绍、使用支持和隐私政策，展示应用实际界面的示例价格截图。

## 本地预览

```sh
python3 -m http.server 4784 --bind 127.0.0.1
```

打开 http://localhost:4784/ 。无需安装依赖或构建。

## 页面

| 页面 | 简体中文 | English |
| --- | --- | --- |
| 产品介绍 | `index.html` | `en/index.html` |
| 使用支持 | `support.html` | `en/support.html` |
| 隐私政策 | `privacy.html` | `en/privacy.html` |

站内导航及图片使用相对路径，兼容 GitHub Pages 仓库子路径和独立域名。图片均为示例价格，页面不接入实时行情；没有分析脚本、外部字体或数据表单。

## GitHub Pages

仓库 Settings → Pages → Build and deployment 选择 **GitHub Actions**。推送 main 后由 `.github/workflows/pages.yml` 发布静态页面。

仅发布六个 HTML 页面、CSS 和图片，不发布说明文档或 Git 配置。

取得正式域名并完成 DNS/HTTPS 后，再增加 CNAME 和对应的语言 alternate/canonical。尚未设置未验证的自定义域名。寸金应用目前处于上架准备阶段，购买入口显示“即将登陆 Mac App Store”，取得正式商店链接后再更新。

## 2026-11-06

- 中英文六页完成，桌面及 390px 窄屏布局检查通过。
- 页面链接及图片资源检查通过。
- 独立项目，不依赖 HiBody 的网站目录和部署。
