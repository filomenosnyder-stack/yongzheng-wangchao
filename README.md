# 雍正王朝（1999）· 素材站

《雍正王朝》超糖卡的图床与视频床。**一张卡一个仓库**，不跟别的作品混放。

线上地址：https://filomenosnyder-stack.github.io/yongzheng-wangchao/

---

## 目录

```
index.html              前端单页（与超糖卡的 description 是同一份）
chars/<拼音>.jpg        28 个角色的头像（384×384，与大明同规格）
chars/poster.jpg        主视觉海报（封面用）
chars/manifest.json     角色清单：中文名 / 拼音 / 排行 / 阵营 / 一句话 / 图片路径
video/si-age-full.mp4   四阿哥 · 九子夺嫡结算 · 7:10 · 960×540 · 20MB
video/ba-xianwang-full.mp4  八贤王 · 「皇上四哥，你赢了」· 2:15 · 720×720 · 9.5MB
```

## 资源怎么引

```js
var ASSET_BASE = "https://filomenosnyder-stack.github.io/yongzheng-wangchao/";
// 图片 -> ASSET_BASE + "chars/" + "<拼音>.jpg"
// 视频 -> ASSET_BASE + "video/" + "<名字>.mp4"
```

卡里改 `ASSET_BASE` 一处即可；留空则走本地相对路径（`../chars/` 与 `assets/`），
方便 file:// 直接预览。

## 28 个角色

| 拼音 | 角色 | 拼音 | 角色 |
|---|---|---|---|
| qiangxi | 康熙 · 圣祖 | wusidao | 邬思道 |
| yinti | 大阿哥 · 胤禔 | zhangtingyu | 张廷玉 |
| yinreng | 二阿哥 · 胤礽 | tongguowei | 佟国维 |
| yinzhi | 三阿哥 · 胤祉 | longkeduo | 隆科多 |
| yongzheng | 四阿哥 · 雍正 | niangengyao | 年羹尧 |
| yinsi | 八阿哥 · 胤禩（八贤王） | tianwenjing | 田文镜 |
| yintang | 九阿哥 · 胤禟 | liwei | 李卫 |
| yine | 十阿哥 · 胤䄉 | lifu | 李绂 |
| yinxiang | 十三阿哥 · 胤祥 | sunjiacheng | 孙嘉诚 |
| yinti2 | 十四阿哥 · 胤禵 | liumolin | 刘墨林 |
| hongshi | 三子 · 弘时 | nuomin | 诺敏 |
| hongli | 四子 · 弘历 | wuya | 乌雅氏 · 德妃 |
| qiaoyindi | 乔引娣 | zhengchunhua | 郑春华 |
| nianqiuyue | 年秋月 | sushunqing | 苏舜卿 |

## 头像怎么来的

豆瓣剧照（约 985 张）→ OpenCV YuNet 检测人脸 → 按最大脸自动裁 384×384 方图 →
用上传者标注的「集数[时间码]角色名」自动归类 → 人工核对。
其中 **雍正 / 胤禩 / 胤禔** 三张为手动指定的图。

⚠ 头像只用于个人自制的非商业同人卡，版权属原剧方。
