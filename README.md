# Typora配置github图床

- 安装 Typora [https://typora.io/](https://typora.io/)

- 安装Typora中的PicGo-Core

    ![Untitled](https://gitee.com/Gwkang/image-host/raw/master/images/2021-08-18_17:11:22.png)

- 安装 Node.js [https://nodejs.org/en/](https://nodejs.org/en/)

- github不支持上传同名文件, 安装super-prefix插件 `C:\Users\admin\AppData\Roaming\Typora\picgo\win64`

    ```bash
    picgo install super-prefix
    ```

- 创建github仓库

    ![image](https://user-images.githubusercontent.com/35400668/130176394-e3bac4e1-8082-4514-81d4-ec0abc65d73a.png)


- 申请token  [https://github.com/settings/tokens](https://github.com/settings/tokens)

    ![image](https://user-images.githubusercontent.com/35400668/130176528-83b4ae92-818d-4eb2-8711-2f5fdffa7946.png)


- 打开Typora配置文件

    ![Untitled](https://gitee.com/Gwkang/image-host/raw/master/images/2021-08-18_17:12:14.png)

- 修改为

```json
{
  "picBed": {
    "current": "github",
    "github": {
      "branch": "main",
      "path": "images/",
      "repo": "iGwkang/imagebed",
      "token": "xxxxxx"
    }
  },
  "picgoPlugins": {
    "picgo-plugin-super-prefix": true
  },
  "picgo-plugin-super-prefix": {
    "prefixFormat": "YYYY/MM/DD/",
    "fileFormat": "HHmmss"
  }
}
```
