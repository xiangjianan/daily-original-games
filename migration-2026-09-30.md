# 历史游戏迁移 · 2026-09-30

**最终状态：8款迁移完成，8个旧仓库全部删除并核实404；完整备份保留。**

将本系列8个独立仓库迁入daily-original-games根日期目录。远程账户仓库清单与原索引交叉核对；daily-games是另一Hermes系列，game-find100也无本系列关联，均不改动。

## 保全

备份根目录：`/Users/xiangjianan/Documents/Codex/game-repository-backups/2026-09-30/`。每款含mirror.git、完整bundle、refs.txt、从bundle恢复的restore/、GitHub元数据JSON；bundle verify和恢复仓库git fsck均成功。前三十日中的最后三款用本地完整对象制作镜像，所有远程分支/tag引用已通过GitHub API逐一核对。每款5个受控文件，复制前核对SHA256，迁移仅替换已知试玩/源码/分享链接和仓库标签。无submodule或LFS。

所有源无issue、PR、release、评论、wiki或独有tag；每款main历史已保全。9/30有两份Pages构建artifact，已下载ZIP并校验，其余无artifact。元数据、fork列表、labels和milestones已保存。

恢复示例：`git clone /备份根/源仓库名/源仓库名.bundle recovered-game`。完整机器清单和文件SHA256见备份根manifest.json。备份保存在本机，不上传GitHub。

## 映射与验证

|源仓库（xiangjianan/）|新目录与试玩|源main提交|备份bundle SHA256|状态|
|---|---|---|---|---|
|daily-original-game-2026-09-16|[2026-09-16/](https://xiangjianan.github.io/daily-original-games/2026-09-16/)|`d34e600c323c40f4a75da3cfb3163f369da79f0a`|`a032e041846dee7063bf53c2467e03dc439e5bb0eeb16898f663d233c746aefd`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|
|daily-original-game-2026-09-23|[2026-09-23/](https://xiangjianan.github.io/daily-original-games/2026-09-23/)|`8b4e589261ea4110e9e5f73b726b1fce7f912b79`|`8b364bee09a7c157decae2c9f4c20ce7d107b3b6f4353e85702d79d3dbf41be2`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|
|daily-original-game-2026-09-24|[2026-09-24/](https://xiangjianan.github.io/daily-original-games/2026-09-24/)|`19ff8d6e914561cd6d71d7061e872ecbb9869c44`|`114a5409d534e2a4249002a5db901ce1b093f41bfa9a8d6f91d88f23f9d33fa1`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|
|daily-original-game-2026-09-25|[2026-09-25/](https://xiangjianan.github.io/daily-original-games/2026-09-25/)|`420e9eaf852e5af05bc599032893bb8344204ca0`|`da230c13a0d46d98ae273aa8d950cf5e2f7a0d260475a786eb9c9757b16152a6`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|
|daily-original-game-2026-09-26|[2026-09-26/](https://xiangjianan.github.io/daily-original-games/2026-09-26/)|`e05c1a635eeed538b6e5c2fb9c07833f75b9ff6b`|`5404d1b4c6075dc1834ddd5b56244c40ce3203e8aa164746c1595e3e7ca5b1a0`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|
|daily-original-game-2026-09-27|[2026-09-27/](https://xiangjianan.github.io/daily-original-games/2026-09-27/)|`aeee939f302eb4fc0a664b3ca1e2eb7d7835a556`|`6eb5068432e348c375baace3a6b53dbf1615d5442973507d27ccb60ce27afda7`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|
|daily-original-game-2026-09-28|[2026-09-28/](https://xiangjianan.github.io/daily-original-games/2026-09-28/)|`676620e1bb6d3cb92d7dc922fbfeda6015ee144e`|`505928b5226ab4744457b42fd775a122c49b9514c74453d66817099e9542badc`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|
|daily-original-game-2026-09-30|[2026-09-30/](https://xiangjianan.github.io/daily-original-games/2026-09-30/)|`28fe76e0022467bee506a260a24e6dfe0a1a1144`|`c1ddb25789f10f1caf5cc07c405adde26c2465ebb8c21517f21bda02de52ea1f`|完整性、备份、本地与线上完整试玩通过；旧源已删除，API 404核实|

## 自动化

automation-2已通过正式automation_update改为本仓库YYYY-MM-DD/index.html和总Pages日期路径，不再新建每日仓库。北京时间12:00、ACTIVE、原通知偏好及研究/原创/音效/分享/真实试玩/文档要求保留，已重新读取配置确认。

## 真实浏览器验证结果

Chrome / Playwright：8款本地与正式HTTPS新路径测试全通过；9/16完成30滴及失败、9/23完成18步及失败、9/24三段通关及步数耗尽、9/25完成12单及三次错误、9/26完成20封及满袋失败、9/27六段1590分及信号耗尽、9/28完成18次及无处可种、9/30完成16箱及超载结束。每款均验证得分、重开、分享、静音。

另独立遍历全部新URL，HTTP200、无失败资源或控制台错误、分享含新路径、390与1280像素无横向溢出；已保存截图并抽查9/16、9/26、9/30手机页面。物理手机、其他浏览器和主观听感未测。原逻辑未改变；仅分享/源码链接修改。

## 首次删除阻塞（历史记录，已解决）

2026-09-30尝试删除已完整迁移并验证的9/16源仓库，首次TLS握手超时；读取确认仍存在后重试，GitHub返回HTTP403：Must have admin rights to Repository，并明确需要delete_repo scope。gh auth status只有repo等权限，无delete_repo。故删除数为0，8个源仓库全部保留。需用户在终端完成 `gh auth refresh -h github.com -s delete_repo` 授权后续做；无需再次确认迁移/删除意图。继续时须重核源提交未变、备份完整及新地址可用，再逐一删除并查不存在。

新总入口及每日自动化已生效；旧仓库与旧Pages目前仍可存在，真正删除后旧链接将失效。

## 删除完成

用户补充delete_repo授权后，于2026-09-30再次逐款检查所有远程分支/tag与提交未变；issue、PR、release、wiki等无新增，附件ZIP与bundle完整性复核通过，新线上HTML与迁移文件逐字节相同。随后严格按8款清单删除，每个DELETE成功并GET返回HTTP404。已删除8/8，无剩余阻塞。总仓库daily-original-games和其他系列未删除。备份全部保留在原路径。确切结果见migration-evidence/2026-09-30/deletion-results.json。
