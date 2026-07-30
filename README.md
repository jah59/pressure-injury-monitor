# 压力性损伤皮肤监护 V1.29｜GitHub Pages 部署说明

本目录已经整理为可直接部署到 GitHub Pages 的静态网站。

## 一、推荐部署方式：从 main 分支根目录发布

1. 登录 GitHub，点击右上角“+”，选择 **New repository**。
2. 输入仓库名称，例如：
   - `pressure-injury-monitor`
   - 或其他英文名称。
3. 建议选择 **Public**，然后点击 **Create repository**。
4. 解压本部署包。
5. 在新仓库中点击 **Add file → Upload files**。
6. 将解压后的所有文件和文件夹上传到仓库根目录：
   - `.nojekyll`
   - `index.html`
   - `assets` 文件夹
   - `README.md`
7. 点击 **Commit changes**。
8. 打开仓库的 **Settings → Pages**。
9. 在 **Build and deployment** 中设置：
   - Source：`Deploy from a branch`
   - Branch：`main`
   - Folder：`/(root)`
10. 点击 **Save**，等待 GitHub Pages 完成发布。

## 二、访问地址

普通项目仓库的地址通常为：

`https://你的GitHub用户名.github.io/仓库名称/`

例如：

`https://example.github.io/pressure-injury-monitor/`

如果仓库名称为：

`你的GitHub用户名.github.io`

访问地址通常为：

`https://你的GitHub用户名.github.io/`

## 三、重要注意事项

- 不要把压缩包本身直接上传到仓库，必须先解压，再上传其中的文件。
- `index.html` 必须位于仓库根目录。
- `assets` 文件夹必须完整保留，不能只上传 `index.html`。
- 文件夹名称和文件名称不要修改，否则背景图片可能无法加载。
- 本项目使用相对路径，可部署在 `用户名.github.io/仓库名/` 子路径下。
- 首次发布或更新后，GitHub Pages 可能需要几分钟才能显示最新内容。
- 如果页面显示404，请检查 Settings → Pages 是否选择了 `main` 和 `/(root)`。
- 如果页面能打开但背景图片缺失，请检查 `assets/backgrounds` 是否完整上传。

## 四、文件结构

```text
/
├─ .nojekyll
├─ index.html
├─ README.md
└─ assets/
   └─ backgrounds/
      ├─ bg_case.png
      ├─ bg_comfort.png
      ├─ bg_environment.png
      ├─ bg_focus_inspect.png
      ├─ bg_item_check.png
      ├─ bg_item_select.png
      ├─ bg_nurse_prepare.png
      ├─ bg_offload.png
      ├─ bg_record.png
      ├─ bg_reposition.png
      ├─ bg_review.png
      ├─ bg_skin_care.png
      ├─ bg_skin_initial.png
      └─ bg_turn_prepare.png
```
