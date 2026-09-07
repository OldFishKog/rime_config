# 说明
只是用来当作操作系统备份

# 步骤
从aur安装rime
```bash
paru -S  rime-ice-git
```
编辑配置文件
```bash
nvim ~/.local/share/fcitx5/rime/default.custom.yaml
```
增加一下内容
```yaml
patch:
  # 引入 AUR 雾凇拼音包附带的默认配置项
  __include: rime_ice_suggestion:/

  # 选定你想要的输入方案
  schema_list:
    - schema: rime_ice

  # 更改每页候选词个数（可选范围 1-9）
  menu/page_size: 9
```