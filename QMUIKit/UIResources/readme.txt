
<QMUIResources.bundle 使用介绍>
QMUIResources.bundle 是QMUI里面使用的图片资源，如果QMUI是作为静态库的方式来引入，图片资源必须打包成一个bundle才能够被访问到。
1、把QMUI拉到所在项目之后，在QMUI的UIResources文件夹里面把bundle文件拉到xcode里面你所在项目的指定目录下（注意是引用，而不是复制一份）。
2、每次更新QMUI的时候，理论上是不需要重新把这个文件拉到跟目录的，因为这里是引用的关系，根目录这里的bundle还是引用了QMUI里面那个bundle。
3、请不要尝试修改这个bundle文件。

<QMUI_QQEmotion.bundle 使用介绍>
QMUI中有个QQ表情的控件，所以需要把所有的QQ表情都打包在bundle里面，建议当项目中需要使用QQ表情控件的时候才去引入这个bundle。

<注意>
如果使用了framework的方式来使用QMUI，则不需要在项目中引入bundle文件，因为bundle文件都到打包在QMUIKit.framework中了。
