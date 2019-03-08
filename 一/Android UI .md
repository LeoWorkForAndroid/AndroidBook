## Android UI


### anim

定义渐变动画的 XML 文件。（属性动画也可以保存在此目录中，但是为了区分这两种类型，属性动画首选 animator/ 目录。）

---

### animator 

用于定义属性动画的 XML 文件

---

### drawable

位图文件（.png、.9.png、.jpg、.gif）或编译为以下 Drawable 资源子类型的 XML 文件：

位图文件
九宫格（可调整大小的位图）
状态列表
形状
动画 Drawable
其他 Drawable

---

###lauout

用于定义用户界面布局的 XML 文件

---

### menu

用于定义应用菜单（如选项菜单、上下文菜单或子菜单）的 XML 文件

---




### mipmap

适用于不同启动器图标密度的 Drawable 文件

---

### values

包含字符串、整型数和颜色等简单值的 XML 文件。

其他 res/ 子目录中的 XML 资源文件是根据 XML 文件名定义单个资源，而目录中的 values/ 文件可描述多个资源。对于此目录中的文件，&lt;resources&gt; 元素的每个子元素均定义一个资源。例如，&lt;string&gt; 元素创建 R.string 资源，&lt;color&gt; 元素创建 R.color 资源。

由于每个资源均用其自己的 XML 元素定义，因此您可以根据自己的需要命名文件，并将不同的资源类型放在一个文件中。但是，为了清晰起见，您可能需要将独特的资源类型放在不同的文件中。 例如，对于可在此目录中创建的资源，下面给出了相应的文件名约定：




#### arrays.xml

用于资源数组（类型化数组）。

#### color.xml

用于定义颜色状态列表的 XML 文件,颜色值。

#### dimens.xml

尺寸值。

#### strings.xml

字符串值。

#### styles.xml

样式。

---

### raw

要以原始形式保存的任意文件。要使用原始 InputStream 打开这些资源，请使用资源 ID（即 R.raw.<em>filename</em>）调用Resources.openRawResource()。

但是，如需访问原始文件名和文件层次结构，则可以考虑将某些资源保存在 assets/ 目录下（而不是 res/raw/）。assets/ 中的文件没有资源 ID，因此您只能使用 AssetManager 读取这些文件。

---

### xml

可以在运行时通过调用 Resources.getXML() 读取的任意 XML 文件。各种 XML 配置文件（如可搜索配置）都必须保存在此处。
