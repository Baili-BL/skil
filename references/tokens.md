# {{skill-name}} — 组件

## 1. 按钮

### 变体

| 变体 | 背景色                   | 文字色                     | 边框                       | 圆角                | 高度                   |
| ---- | ------------------------ | -------------------------- | -------------------------- | ------------------- | ---------------------- |
| 主要 | `{{btn-primary-bg}}`     | `{{btn-primary-text}}`     | {{btn-primary-border}}     | {{radii-buttons}}px | {{btn-height}}px       |
| 次要 | `{{btn-secondary-bg}}`   | `{{btn-secondary-text}}`   | {{btn-secondary-border}}   | {{radii-buttons}}px | {{btn-height}}px       |
| 幽灵 | 透明                     | `{{btn-ghost-text}}`       | 无                         | {{radii-buttons}}px | {{btn-ghost-height}}px |
| 危险 | `{{btn-destructive-bg}}` | `{{btn-destructive-text}}` | {{btn-destructive-border}} | {{radii-buttons}}px | {{btn-height}}px       |

### 规格

| 属性         | 值                                                          |
| ------------ | ----------------------------------------------------------- |
| 高度（大）   | {{btn-height}}px                                            |
| 高度（小）   | {{btn-height-small}}px                                      |
| 内边距（大） | {{btn-padding-v}}px {{btn-padding-h}}px                     |
| 内边距（小） | {{btn-padding-v-small}}px {{btn-padding-h-small}}px         |
| 字体         | `{{font-body-name}}` {{btn-font-weight}}，{{btn-font-size}} |
| 最小触控目标 | 44px                                                        |

### 状态

| 状态            | 变化                   |
| --------------- | ---------------------- |
| **悬停**        | {{btn-state-hover}}    |
| **激活 / 按下** | {{btn-state-active}}   |
| **禁用**        | {{btn-state-disabled}} |
| **聚焦**        | {{btn-state-focus}}    |

---

## 2. 卡片 / 表面

### 标准卡片

- 背景：`--surface1`
- 边框：{{border-cards}}
- 圆角：{{radii-cards}}px {{corner-style-note-short}}
- 内边距：{{card-padding}}px
- 阴影：{{shadow-1-light}}（亮色）/ {{shadow-1-dark}}（暗色）

### 特色卡片

- 背景：`--surface1` + {{card-featured-treatment}}
- 圆角：{{radii-cards-featured}}px
- 阴影：{{shadow-2-light}}（亮色）/ {{shadow-2-dark}}（暗色）

### 紧凑卡片

- 圆角：{{radii-cards-compact}}px
- 内边距：{{card-padding-compact}}px
- 背景和边框与标准卡片相同

### 内容布局

- 标题：`--subheading`，`--text1`
- 描述：`--body-sm`，`--text2`
- 元数据：`--caption`，`--text3`
- 元素间内部间距：`--space-sm`
- 按下状态：{{card-press-state}}

---

## 3. 输入框

### 文本输入框

| 属性         | 值                                          |
| ------------ | ------------------------------------------- |
| 高度         | {{input-height}}px                          |
| 背景         | `{{input-bg}}`                              |
| 边框（默认） | {{input-border-default}}                    |
| 边框（聚焦） | {{input-border-focus}}                      |
| 边框（错误） | {{input-border-error}}                      |
| 圆角         | {{radii-inputs}}px                          |
| 内边距       | {{input-padding-v}}px {{input-padding-h}}px |
| 字体         | `{{font-body-name}}`，`--body`              |
| 占位符颜色   | `--text3`                                   |

### 标签

- 位置：字段上方，间距 {{input-label-gap}}px
- 字体：`{{font-body-name}}`，`--body-sm`，`--text2`

### 状态

| 状态     | 处理方式                                                                |
| -------- | ----------------------------------------------------------------------- |
| **默认** | {{input-border-default}}                                                |
| **聚焦** | {{input-border-focus}}。{{input-focus-extra}}                           |
| **错误** | {{input-border-error}}。错误文字显示在下方，使用 `--error`，`--caption` |
| **禁用** | 透明度 0.4，无交互                                                      |

### 多行输入

- 样式与文本输入框相同，最小高度 100px，自动增长

---

## 4. 列表 / 数据行

### 标准行

| 属性     | 值                                                |
| -------- | ------------------------------------------------- |
| 最小高度 | {{list-row-height}}px                             |
| 内边距   | {{list-row-padding-v}}px {{list-row-padding-h}}px |
| 分割线   | {{list-divider}}                                  |
| 标签字体 | `{{font-body-name}}`，`--body`，`--text1`         |
| 值字体   | {{list-value-font}}                               |
| 附件     | {{list-accessory}}                                |

### 交互状态

| 状态     | 处理方式              |
| -------- | --------------------- |
| **默认** | 透明背景              |
| **按下** | {{list-row-pressed}}  |
| **选中** | {{list-row-selected}} |

### 数据行（标签 + 值）

- 左侧：标签，使用 `--text2`
- 右侧：值，使用 `--text1`，{{list-data-value-font}}
- 单位/后缀：`--caption`，`--text3`，紧邻值显示

---

## 5. 导航 / 标签栏

### 标签栏

| 属性 | 值                                |
| ---- | --------------------------------- |
| 高度 | {{nav-tab-height}}px + 安全区域   |
| 背景 | `{{nav-tab-bg}}`                  |
| 边框 | {{nav-tab-border}}                |
| 字体 | `{{font-body-name}}`，`--caption` |

### 标签状态

| 状态       | 处理方式             |
| ---------- | -------------------- |
| **激活**   | {{nav-tab-active}}   |
| **非激活** | {{nav-tab-inactive}} |
| **悬停**   | {{nav-tab-hover}}    |

### 导航栏

- 标题：`--heading`，`--text1`
- 返回按钮：{{nav-back-button}}
- 背景：{{nav-bar-bg}}

---

## 6. 标签 / 芯片

| 属性     | 值                                                     |
| -------- | ------------------------------------------------------ |
| 高度     | {{tag-height}}px                                       |
| 内边距   | {{tag-padding-v}}px {{tag-padding-h}}px                |
| 圆角     | {{radii-tags}}px                                       |
| 字体     | `{{font-body-name}}`，`--caption`，{{tag-font-weight}} |
| 背景     | `{{tag-bg}}`                                           |
| 文字颜色 | `{{tag-text}}`                                         |
| 边框     | {{border-tags}}                                        |

### 选中状态

- 背景：`--accent-subtle`
- 文字：`--accent`
- 边框：{{tag-selected-border}}

### 状态变体

对语义标签使用状态颜色：`--success-bg` + `--success`，`--warning-bg` + `--warning`，`--error-bg` + `--error`。

---

## 7. 浮层

### 模态框 / 对话框

| 属性     | 值                                                    |
| -------- | ----------------------------------------------------- |
| 背景     | `--surface1`                                          |
| 圆角     | {{radii-modals}}px                                    |
| 阴影     | {{shadow-3-light}}（亮色）/ {{shadow-3-dark}}（暗色） |
| 遮罩层   | {{overlay-backdrop}}                                  |
| 最大宽度 | {{overlay-modal-max-width}}px                         |
| 内边距   | {{overlay-modal-padding}}px                           |
| 关闭按钮 | {{overlay-close-button}}                              |

### 底部弹出

| 属性     | 值                   |
| -------- | -------------------- |
| 背景     | `--surface1`         |
| 顶部圆角 | {{radii-modals}}px   |
| 把手     | {{sheet-handle}}     |
| 遮罩层   | {{overlay-backdrop}} |
| 关闭方式 | 下拉关闭             |

### 下拉菜单 / 气泡框

| 属性       | 值                                                    |
| ---------- | ----------------------------------------------------- |
| 背景       | `--surface1`                                          |
| 圆角       | {{radii-dropdown}}px                                  |
| 阴影       | {{shadow-2-light}}（亮色）/ {{shadow-2-dark}}（暗色） |
| 边框       | {{border-dropdown}}                                   |
| 条目高度   | {{dropdown-item-height}}px                            |
| 选中指示器 | {{dropdown-selected}}                                 |

---

## 8. 状态模式

### 空状态

- 布局：居中，顶部留白充分（{{empty-state-top-padding}}px+）
- 图标/插图：{{empty-state-icon}}
- 标题：`--subheading`，`--text2`
- 描述：`--body`，`--text3`，最多两行
- CTA：主要按钮，距描述 {{empty-state-cta-gap}}px

### 加载中

- 行内：{{loading-inline}}
- 全屏：{{loading-fullscreen}}
- 内容出现：{{loading-content-transition}}

### 错误

- 行内（字段）：`--error` 文字，使用 `--caption` 显示在元素下方
- 屏幕级：{{error-screen-level}}
- 语气：{{error-tone}}

### 禁用

- 透明度 0.4，无交互，保持布局
- 边框淡化为 `--border` 默认值
- 无悬停/聚焦状态

---

## 9. 开关

### 规格

| 属性         | 值                                        |
| ------------ | ----------------------------------------- |
| 轨道宽度     | {{toggle-track-width}}px                  |
| 轨道高度     | {{toggle-track-height}}px                 |
| 轨道圆角     | {{toggle-track-radius}}px                 |
| 滑块尺寸     | {{toggle-thumb-size}}px                   |
| 滑块圆角     | {{toggle-thumb-radius}}px                 |
| 滑块距边偏移 | {{toggle-thumb-offset}}px                 |
| 标签位置     | {{toggle-label-position}}                 |
| 标签间距     | {{toggle-label-gap}}px                    |
| 标签字体     | `{{font-body-name}}`，`--body`，`--text1` |

### 状态

| 状态           | 轨道背景                  | 滑块                   |
| -------------- | ------------------------- | ---------------------- |
| **关（默认）** | `{{toggle-track-off-bg}}` | `{{toggle-thumb-off}}` |
| **开**         | `{{toggle-track-on-bg}}`  | `{{toggle-thumb-on}}`  |
| **悬停**       | {{toggle-state-hover}}    | —                      |
| **禁用**       | 透明度 0.4，无交互        | —                      |
| **聚焦**       | {{toggle-state-focus}}    | —                      |

---

## 10. 复选框

### 规格

| 属性           | 值                                        |
| -------------- | ----------------------------------------- |
| 尺寸           | {{checkbox-size}}px                       |
| 边框（未选中） | {{checkbox-border}}                       |
| 圆角           | {{checkbox-radius}}px                     |
| 选中填充       | `{{checkbox-checked-bg}}`                 |
| 勾选标记颜色   | `{{checkbox-checkmark-color}}`            |
| 勾选标记描边   | {{checkbox-checkmark-stroke}}px           |
| 标签间距       | {{checkbox-label-gap}}px                  |
| 标签字体       | `{{font-body-name}}`，`--body`，`--text1` |

### 变体

| 变体   | 处理方式                                                                |
| ------ | ----------------------------------------------------------------------- |
| 未选中 | {{checkbox-border}}，透明填充                                           |
| 已选中 | `{{checkbox-checked-bg}}` 填充，`{{checkbox-checkmark-color}}` 勾选标记 |
| 不确定 | `{{checkbox-checked-bg}}` 填充，`{{checkbox-checkmark-color}}` 横杠     |

### 状态

| 状态     | 处理方式                  |
| -------- | ------------------------- |
| **默认** | {{checkbox-border}}       |
| **悬停** | {{checkbox-state-hover}}  |
| **激活** | {{checkbox-state-active}} |
| **禁用** | 透明度 0.4，无交互        |
| **聚焦** | {{checkbox-state-focus}}  |

---

## 11. 单选按钮

### 规格

| 属性       | 值                                                                |
| ---------- | ----------------------------------------------------------------- |
| 尺寸       | {{radio-size}}px                                                  |
| 边框       | {{radio-border}}                                                  |
| 圆角       | 50%（圆形）                                                       |
| 选中指示器 | {{radio-indicator-size}}px 圆点，使用 `{{radio-indicator-color}}` |
| 选中边框   | {{radio-selected-border}}                                         |
| 标签间距   | {{radio-label-gap}}px                                             |
| 标签字体   | `{{font-body-name}}`，`--body`，`--text1`                         |

### 状态

| 状态     | 处理方式                                                        |
| -------- | --------------------------------------------------------------- |
| **默认** | {{radio-border}}，透明填充                                      |
| **已选** | {{radio-selected-border}}，内部圆点 `{{radio-indicator-color}}` |
| **悬停** | {{radio-state-hover}}                                           |
| **禁用** | 透明度 0.4，无交互                                              |
| **聚焦** | {{radio-state-focus}}                                           |

---

## 12. 滑块 / 范围选择

### 规格

| 属性               | 值                           |
| ------------------ | ---------------------------- |
| 轨道高度           | {{slider-track-height}}px    |
| 轨道圆角           | {{slider-track-radius}}px    |
| 轨道背景（未填充） | `{{slider-track-bg}}`        |
| 轨道背景（已填充） | `{{slider-track-filled-bg}}` |
| 滑块宽度           | {{slider-thumb-width}}px     |
| 滑块高度           | {{slider-thumb-height}}px    |
| 滑块圆角           | {{slider-thumb-radius}}px    |
| 滑块背景           | `{{slider-thumb-bg}}`        |
| 滑块边框           | {{slider-thumb-border}}      |
| 刻度标记           | {{slider-step-marks}}        |
| 值标签             | {{slider-value-label}}       |

### 状态

| 状态              | 处理方式                |
| ----------------- | ----------------------- |
| **默认**          | 按规格显示              |
| **悬停**          | {{slider-state-hover}}  |
| **激活 / 拖动中** | {{slider-state-active}} |
| **禁用**          | 透明度 0.4，无交互      |
| **聚焦**          | {{slider-state-focus}}  |

---

## 13. 下拉选择 / 触发器

### 规格

| 属性       | 值                                          |
| ---------- | ------------------------------------------- |
| 高度       | {{input-height}}px（继承自输入框）          |
| 背景       | `{{input-bg}}`                              |
| 边框       | {{input-border-default}}                    |
| 圆角       | {{radii-inputs}}px                          |
| 内边距     | {{input-padding-v}}px {{input-padding-h}}px |
| 字体       | `{{font-body-name}}`，`--body`，`--text1`   |
| 占位符颜色 | `--text3`                                   |
| 下箭头图标 | {{select-chevron-icon}}                     |
| 下箭头颜色 | `--text3`                                   |
| 下箭头尺寸 | {{select-chevron-size}}px                   |

### 状态

| 状态     | 处理方式                                                             |
| -------- | -------------------------------------------------------------------- |
| **默认** | {{input-border-default}}，箭头朝下                                   |
| **悬停** | {{select-state-hover}}                                               |
| **展开** | {{input-border-focus}}，箭头旋转 180 度。下拉菜单参见浮层 > 下拉菜单 |
| **禁用** | 透明度 0.4，无交互                                                   |
| **聚焦** | {{input-border-focus}}。{{input-focus-extra}}                        |
| **错误** | {{input-border-error}}                                               |

---

## 14. 多行文本框

继承**输入框 > 文本输入框**的所有样式，并做以下覆盖：

| 属性         | 值                                           |
| ------------ | -------------------------------------------- |
| 最小高度     | {{textarea-min-height}}px                    |
| 调整行为     | {{textarea-resize}}                          |
| 行高         | {{textarea-line-height}}                     |
| 内边距       | {{textarea-padding}}px                       |
| 字数统计位置 | {{textarea-char-count-position}}             |
| 字数统计字体 | `{{font-body-name}}`，`--caption`，`--text3` |

### 状态

与输入框相同（默认、聚焦、错误、禁用）。

---

## 15. 数据表格

### 表头行

| 属性         | 值                                                                         |
| ------------ | -------------------------------------------------------------------------- |
| 高度         | {{table-header-height}}px                                                  |
| 背景         | `{{table-header-bg}}`                                                      |
| 字体         | `{{font-body-name}}`，`--caption`，{{table-header-font-weight}}，`--text2` |
| 文字转换     | {{table-header-text-transform}}                                            |
| 单元格内边距 | {{table-cell-padding-v}}px {{table-cell-padding-h}}px                      |
| 排序指示器   | {{table-sort-indicator}}                                                   |
| 底部边框     | {{table-header-border}}                                                    |

### 数据行

| 属性         | 值                                                    |
| ------------ | ----------------------------------------------------- |
| 高度         | {{table-row-height}}px                                |
| 字体         | `{{font-body-name}}`，`--body`，`--text1`             |
| 单元格内边距 | {{table-cell-padding-v}}px {{table-cell-padding-h}}px |
| 行分割线     | {{table-row-divider}}                                 |
| 列对齐       | {{table-column-alignment}}                            |

### 行状态

| 状态               | 处理方式               |
| ------------------ | ---------------------- |
| **默认**           | 透明背景               |
| **悬停**           | {{table-row-hover}}    |
| **已选**           | {{table-row-selected}} |
| **斑马纹（可选）** | {{table-row-striped}}  |

---

## 16. 选项卡

### 规格

| 属性         | 值                                                      |
| ------------ | ------------------------------------------------------- |
| 栏高度       | {{tabs-bar-height}}px                                   |
| 选项卡内边距 | {{tabs-tab-padding-v}}px {{tabs-tab-padding-h}}px       |
| 字体         | `{{font-body-name}}`，`--body-sm`，{{tabs-font-weight}} |
| 选项卡间距   | {{tabs-gap}}px                                          |
| 激活指示器   | {{tabs-active-indicator}}                               |
| 栏边框       | {{tabs-bar-border}}                                     |
| 过渡         | {{tabs-transition}}                                     |

### 状态

| 状态       | 处理方式                                        |
| ---------- | ----------------------------------------------- |
| **激活**   | {{tabs-active-text}}，{{tabs-active-indicator}} |
| **非激活** | {{tabs-inactive-text}}                          |
| **悬停**   | {{tabs-hover}}                                  |
| **禁用**   | 透明度 0.4，无交互                              |
| **聚焦**   | {{tabs-focus}}                                  |

---

## 17. 面包屑

### 规格

| 属性       | 值                                        |
| ---------- | ----------------------------------------- |
| 字体       | `{{font-body-name}}`，`--body-sm`         |
| 链接颜色   | `--text2`                                 |
| 链接悬停   | {{breadcrumb-link-hover}}                 |
| 分隔符     | {{breadcrumb-separator}}                  |
| 分隔符颜色 | `--text3`                                 |
| 分隔符间距 | 两侧各 {{breadcrumb-separator-spacing}}px |
| 当前页     | {{breadcrumb-current-page}}               |

---

## 18. 头像

### 尺寸

| 尺寸 | 尺寸值               | 字体（首字母） |
| ---- | -------------------- | -------------- |
| 小   | {{avatar-size-sm}}px | `--caption`    |
| 中   | {{avatar-size-md}}px | `--body-sm`    |
| 大   | {{avatar-size-lg}}px | `--body`       |

### 规格

| 属性         | 值                              |
| ------------ | ------------------------------- |
| 圆角         | {{avatar-radius}}               |
| 回退背景     | `{{avatar-fallback-bg}}`        |
| 回退文字颜色 | `{{avatar-fallback-text}}`      |
| 回退字重     | {{avatar-fallback-font-weight}} |
| 边框         | {{avatar-border}}               |
| 状态点尺寸   | {{avatar-status-dot-size}}px    |
| 状态点位置   | {{avatar-status-dot-position}}  |
| 状态点边框   | {{avatar-status-dot-border}}    |

### 状态点颜色

| 状态 | 颜色        |
| ---- | ----------- |
| 在线 | `--success` |
| 离开 | `--warning` |
| 离线 | `--text3`   |
| 忙碌 | `--error`   |

---

## 19. 徽章 / 状态点

### 规格

| 属性           | 值                                                       |
| -------------- | -------------------------------------------------------- |
| 高度           | {{badge-height}}px                                       |
| 最小宽度       | {{badge-min-width}}px                                    |
| 内边距         | {{badge-padding-v}}px {{badge-padding-h}}px              |
| 圆角           | {{badge-radius}}px                                       |
| 字体           | `{{font-body-name}}`，`--caption`，{{badge-font-weight}} |
| 相对父元素位置 | {{badge-position}}                                       |

### 语义变体

| 变体 | 背景                   | 文字                     |
| ---- | ---------------------- | ------------------------ |
| 中性 | `{{badge-neutral-bg}}` | `{{badge-neutral-text}}` |
| 成功 | `--success-bg`         | `--success`              |
| 警告 | `--warning-bg`         | `--warning`              |
| 错误 | `--error-bg`           | `--error`                |
| 信息 | `{{badge-info-bg}}`    | `{{badge-info-text}}`    |

### 状态点（仅图标）

- 尺寸：{{badge-dot-size}}px
- 与徽章相同的语义颜色映射，无文字
- 边框：{{badge-dot-border}}

---

## 20. 工具提示

### 规格

| 属性     | 值                                              |
| -------- | ----------------------------------------------- |
| 背景     | `{{tooltip-bg}}`                                |
| 文字颜色 | `{{tooltip-text}}`                              |
| 字体     | `{{font-body-name}}`，`--caption`               |
| 圆角     | {{tooltip-radius}}px                            |
| 内边距   | {{tooltip-padding-v}}px {{tooltip-padding-h}}px |
| 最大宽度 | {{tooltip-max-width}}px                         |
| 箭头     | {{tooltip-arrow}}                               |
| 显示延迟 | {{tooltip-delay-show}}ms                        |
| 隐藏延迟 | {{tooltip-delay-hide}}ms                        |
| 位置     | {{tooltip-placement}}                           |
| 阴影     | {{tooltip-shadow}}                              |

---

## 21. 提示条 / 横幅

### 规格

| 属性         | 值                                                             |
| ------------ | -------------------------------------------------------------- |
| 圆角         | {{alert-radius}}px                                             |
| 内边距       | {{alert-padding}}px                                            |
| 图标尺寸     | {{alert-icon-size}}px                                          |
| 图标间距     | {{alert-icon-gap}}px                                           |
| 字体（标题） | `{{font-body-name}}`，`--body-sm`，{{alert-title-font-weight}} |
| 字体（描述） | `{{font-body-name}}`，`--body-sm`，`--text2`                   |
| 关闭按钮     | {{alert-dismiss}}                                              |
| 布局         | {{alert-layout}}                                               |

### 语义变体

| 变体 | 背景                | 边框                     | 图标颜色              | 文字颜色  |
| ---- | ------------------- | ------------------------ | --------------------- | --------- |
| 信息 | `{{alert-info-bg}}` | {{alert-info-border}}    | `{{alert-info-icon}}` | `--text1` |
| 成功 | `--success-bg`      | {{alert-success-border}} | `--success`           | `--text1` |
| 警告 | `--warning-bg`      | {{alert-warning-border}} | `--warning`           | `--text1` |
| 错误 | `--error-bg`        | {{alert-error-border}}   | `--error`             | `--text1` |

---

## 22. Toast / 通知

### 规格

| 属性       | 值                                |
| ---------- | --------------------------------- |
| 位置       | {{toast-position}}                |
| 最大宽度   | {{toast-max-width}}px             |
| 背景       | `{{toast-bg}}`                    |
| 文字颜色   | `{{toast-text}}`                  |
| 圆角       | {{toast-radius}}px                |
| 内边距     | {{toast-padding}}px               |
| 阴影       | {{toast-shadow}}                  |
| 字体       | `{{font-body-name}}`，`--body-sm` |
| 自动关闭   | {{toast-auto-dismiss}}ms          |
| 动画       | {{toast-animation}}               |
| 关闭按钮   | {{toast-dismiss}}                 |
| 最大堆叠数 | {{toast-max-stack}}               |

### 语义变体

| 变体 | 强调色 / 图标颜色 |
| ---- | ----------------- |
| 中性 | `--text2`         |
| 成功 | `--success`       |
| 警告 | `--warning`       |
| 错误 | `--error`         |

---

## 23. 进度条

### 规格

| 属性       | 值                                           |
| ---------- | -------------------------------------------- |
| 高度       | {{progress-height}}px                        |
| 轨道圆角   | {{progress-radius}}px                        |
| 轨道背景   | `{{progress-track-bg}}`                      |
| 填充颜色   | `{{progress-fill-color}}`                    |
| 填充圆角   | {{progress-radius}}px                        |
| 标签位置   | {{progress-label-position}}                  |
| 标签字体   | `{{font-body-name}}`，`--caption`，`--text2` |
| 不确定动画 | {{progress-indeterminate-animation}}         |

### 语义填充颜色

| 变体 | 填充        |
| ---- | ----------- |
| 默认 | `--accent`  |
| 成功 | `--success` |
| 警告 | `--warning` |
| 错误 | `--error`   |

---

## 24. 加载指示器

### 规格

| 属性       | 值                         |
| ---------- | -------------------------- |
| 尺寸（小） | {{spinner-size-sm}}px      |
| 尺寸（中） | {{spinner-size-md}}px      |
| 尺寸（大） | {{spinner-size-lg}}px      |
| 描边宽度   | {{spinner-stroke-width}}px |
| 颜色       | `{{spinner-color}}`        |
| 轨道颜色   | `{{spinner-track-color}}`  |
| 动画       | {{spinner-animation}}      |

---

## 25. 骨架屏

### 规格

| 属性     | 值                                |
| -------- | --------------------------------- |
| 背景     | `{{skeleton-bg}}`                 |
| 闪光颜色 | `{{skeleton-shimmer}}`            |
| 圆角     | 匹配目标组件圆角                  |
| 动画     | {{skeleton-animation}}            |
| 动画时长 | {{skeleton-animation-duration}}ms |

### 常见形状

| 形状         | 尺寸                                | 圆角                        |
| ------------ | ----------------------------------- | --------------------------- |
| 文本行       | 100% x {{skeleton-text-height}}px   | {{skeleton-text-radius}}px  |
| 标题         | 60% x {{skeleton-heading-height}}px | {{skeleton-text-radius}}px  |
| 圆形（头像） | {{avatar-size-md}}px                | 50%                         |
| 矩形（卡片） | 100% x {{skeleton-card-height}}px   | {{radii-cards}}px           |
| 缩略图       | {{skeleton-thumb-size}}px           | {{skeleton-thumb-radius}}px |

---

## 26. 折叠面板

### 规格

| 属性           | 值                                                                          |
| -------------- | --------------------------------------------------------------------------- |
| 标题高度       | {{accordion-header-height}}px                                               |
| 标题内边距     | {{accordion-header-padding-v}}px {{accordion-header-padding-h}}px           |
| 标题字体       | `{{font-body-name}}`，`--body`，{{accordion-header-font-weight}}，`--text1` |
| 箭头图标尺寸   | {{accordion-chevron-size}}px                                                |
| 箭头图标颜色   | `--text3`                                                                   |
| 展开时箭头旋转 | 180度                                                                       |
| 内容内边距     | {{accordion-content-padding}}px                                             |
| 内容字体       | `{{font-body-name}}`，`--body`，`--text2`                                   |
| 分割线         | {{accordion-divider}}                                                       |
| 背景           | {{accordion-bg}}                                                            |
| 圆角           | {{accordion-radius}}px                                                      |

### 状态

| 状态     | 处理方式                  |
| -------- | ------------------------- |
| **收起** | 箭头朝下，内容隐藏        |
| **展开** | 箭头旋转 180 度，内容可见 |
| **悬停** | {{accordion-state-hover}} |
| **禁用** | 透明度 0.4，无交互        |
| **聚焦** | {{accordion-state-focus}} |

---

## 27. 图表容器

### 规格

| 属性         | 值                           |
| ------------ | ---------------------------- |
| 背景         | {{chart-container-bg}}       |
| 边框         | {{chart-container-border}}   |
| 圆角         | {{chart-container-radius}}px |
| 内边距       | {{chart-container-padding}}  |
| 标题字体     | {{chart-title-font}}         |
| 描述字体     | {{chart-description-font}}   |
| 操作按钮位置 | {{chart-actions-position}}   |

### 布局

- 标题区：标题（左）+ 操作按钮（右）
- 描述区：副标题或说明文字
- 图表区：主可视化区域
- 图例区：底部或右侧

---

## 28. 轴标签

### 规格

| 属性        | 值                      |
| ----------- | ----------------------- |
| 字体        | {{axis-label-font}}     |
| 颜色        | {{axis-label-color}}    |
| X轴标签旋转 | {{axis-label-rotation}} |
| 标签间距    | {{axis-label-gap}}px    |
| 网格线颜色  | {{axis-grid-color}}     |
| 网格线样式  | {{axis-grid-style}}     |

---

## 29. 图例

### 规格

| 属性       | 值                         |
| ---------- | -------------------------- |
| 布局方向   | {{legend-direction}}       |
| 色块尺寸   | {{legend-swatch-size}}px   |
| 色块圆角   | {{legend-swatch-radius}}px |
| 标签字体   | {{legend-label-font}}      |
| 标签颜色   | {{legend-label-color}}     |
| 项间距     | {{legend-item-gap}}px      |
| 与图表间距 | {{legend-chart-gap}}px     |

### 交互

| 状态       | 处理方式            |
| ---------- | ------------------- |
| **悬停**   | {{legend-hover}}    |
| **禁用项** | {{legend-disabled}} |

---

## 30. 数据工具提示

### 规格

| 属性     | 值                           |
| -------- | ---------------------------- |
| 背景     | {{data-tooltip-bg}}          |
| 边框     | {{data-tooltip-border}}      |
| 圆角     | {{data-tooltip-radius}}px    |
| 内边距   | {{data-tooltip-padding}}     |
| 阴影     | {{data-tooltip-shadow}}      |
| 标题字体 | {{data-tooltip-title-font}}  |
| 数值字体 | {{data-tooltip-value-font}}  |
| 数值颜色 | {{data-tooltip-value-color}} |

### 内容格式

- 系列名称 + 色块
- 数值（等宽字体）
- 百分比（可选）
- 时间/维度标签

---

## 31. 筛选器栏

### 规格

| 属性   | 值                      |
| ------ | ----------------------- |
| 背景   | {{filter-bar-bg}}       |
| 边框   | {{filter-bar-border}}   |
| 圆角   | {{filter-bar-radius}}px |
| 内边距 | {{filter-bar-padding}}  |
| 项间距 | {{filter-item-gap}}px   |

### 筛选器项

| 类型     | 样式                      |
| -------- | ------------------------- |
| 下拉选择 | {{filter-dropdown-style}} |
| 日期选择 | {{filter-date-style}}     |
| 搜索输入 | {{filter-search-style}}   |
| 标签筛选 | {{filter-tag-style}}      |
| 清除按钮 | {{filter-clear-style}}    |

---

## 32. 时间范围选择器

### 规格

| 属性       | 值                      |
| ---------- | ----------------------- |
| 预设选项   | {{time-presets}}        |
| 自定义范围 | {{time-custom-enabled}} |
| 日期格式   | {{time-date-format}}    |
| 快捷选项   | {{time-shortcuts}}      |

### 样式

| 元素       | 值                             |
| ---------- | ------------------------------ |
| 按钮组背景 | {{time-selector-bg}}           |
| 激活项背景 | {{time-selector-active-bg}}    |
| 激活项颜色 | {{time-selector-active-color}} |
| 边框       | {{time-selector-border}}       |
| 圆角       | {{time-selector-radius}}px     |

---

## 33. 颜色比例尺展示

### 规格

| 属性       | 值                       |
| ---------- | ------------------------ |
| 渐变条高度 | {{scale-bar-height}}px   |
| 渐变条宽度 | {{scale-bar-width}}px    |
| 渐变条圆角 | {{scale-bar-radius}}px   |
| 标签字体   | {{scale-label-font}}     |
| 标签位置   | {{scale-label-position}} |
| 标签格式   | {{scale-label-format}}   |

### 类型

| 类型     | 展示方式             |
| -------- | -------------------- |
| 连续渐变 | {{scale-continuous}} |
| 离散分段 | {{scale-discrete}}   |
| 两端标签 | {{scale-end-labels}} |

---

## 34. KPI 卡片

### 规格

| 属性     | 值                    |
| -------- | --------------------- |
| 背景     | {{kpi-card-bg}}       |
| 边框     | {{kpi-card-border}}   |
| 圆角     | {{kpi-card-radius}}px |
| 内边距   | {{kpi-card-padding}}  |
| 图标位置 | {{kpi-icon-position}} |
| 图标尺寸 | {{kpi-icon-size}}px   |

### 内容

| 元素       | 字体               | 颜色                                            |
| ---------- | ------------------ | ----------------------------------------------- |
| 指标名称   | {{kpi-label-font}} | {{kpi-label-color}}                             |
| 主数值     | {{kpi-value-font}} | {{kpi-value-color}}                             |
| 变化指示器 | {{kpi-delta-font}} | {{kpi-delta-positive}} / {{kpi-delta-negative}} |
| 时间标签   | {{kpi-time-font}}  | {{kpi-time-color}}                              |

---

## 35. 数据表格（可视化场景）

### 规格

继承**标准表格**样式，并添加：

| 属性       | 值                         |
| ---------- | -------------------------- |
| 行高       | {{viz-table-row-height}}px |
| 斑马纹     | {{viz-table-striped}}      |
| 悬停高亮   | {{viz-table-hover}}        |
| 选中行     | {{viz-table-selected}}     |
| 排序指示器 | {{viz-table-sort-icon}}    |
| 进度条列   | {{viz-table-progress}}     |
| 趋势图列   | {{viz-table-sparkline}}    |

### 单元格内容

| 类型     | 样式                   |
| -------- | ---------------------- |
| 数值     | {{viz-cell-number}}    |
| 状态徽章 | {{viz-cell-badge}}     |
| 迷你图   | {{viz-cell-sparkline}} |
| 操作按钮 | {{viz-cell-actions}}   |

---

## 36. 空数据状态

### 规格

| 属性     | 值                          |
| -------- | --------------------------- |
| 背景     | {{empty-state-bg}}          |
| 边框     | {{empty-state-border}}      |
| 圆角     | {{empty-state-radius}}px    |
| 内边距   | {{empty-state-padding}}     |
| 图标     | {{empty-state-icon}}        |
| 图标尺寸 | {{empty-state-icon-size}}px |
| 图标颜色 | {{empty-state-icon-color}}  |

### 内容

| 元素     | 字体                       | 颜色                        |
| -------- | -------------------------- | --------------------------- |
| 标题     | {{empty-state-title-font}} | {{empty-state-title-color}} |
| 描述     | {{empty-state-desc-font}}  | {{empty-state-desc-color}}  |
| 操作按钮 | {{empty-state-cta-style}}  | -                           |

---

## 37. 数据标注

### 规格

| 属性   | 值                      |
| ------ | ----------------------- |
| 字体   | {{data-label-font}}     |
| 颜色   | {{data-label-color}}    |
| 背景   | {{data-label-bg}}       |
| 边框   | {{data-label-border}}   |
| 圆角   | {{data-label-radius}}px |
| 内边距 | {{data-label-padding}}  |
| 引线   | {{data-label-leader}}   |

### 位置

| 位置 | 使用场景                   |
| ---- | -------------------------- |
| 顶部 | {{label-position-top}}     |
| 内部 | {{label-position-inside}}  |
| 外部 | {{label-position-outside}} |

### 内容

- 数值（等宽字体）
- 百分比
- 类别名称
- 变化指示（+/-）
