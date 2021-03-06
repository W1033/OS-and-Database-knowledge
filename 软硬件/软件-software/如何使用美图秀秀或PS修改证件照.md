# 如何使用美图秀秀或 PS 修改证件照




## 0. 证件照的要求
一般需要上传证件照的网站, 对证件照的要求主要有 2 点
+ (1) 尺寸为 `358 * 441`px
+ (2) 大小不能超过 20kb

## 1. 使用美图秀秀修改证件照
1. 打开美图秀秀，把图片拉入到主窗口， 点击下图中的 `尺寸`

<img src="./images-software/image-20210207143447846.png"
    style="margin-left: 0; border-radius: 4px; width: 76%;
        box-shadow: 1px 1px 3px 2px #e5e5e5">

2. 在当前的弹框中输入 `358 * 441` ，单位选择 `像素`，把 `锁定长度比例` 取消， 然后点击 `确定`。图示如下：

<img src="./images-software/image-20210207143847484.png"
    style="margin-left: 0; border-radius: 4px; width: 76%;
        box-shadow: 1px 1px 3px 2px #e5e5e5">

3. 然后点击当前窗口右上角的 `保存` 按钮， 在弹出窗口中 `画质调整` 中滑动按钮，来调节要保存图片的大小， 画质越高图片越大，反之越小。图示如下：

<img src="./images-software/image-20210207144410320.png"
    style="margin-left: 0; border-radius: 4px; width: 76%;
        box-shadow: 1px 1px 3px 2px #e5e5e5">



## 2. 使用 PS 修改证件照
上面已经可以使用美图秀秀修改证件照了, 那为什么还要使用 PS 呢? 答: 因为 PS 可以修改的地方更多, 假如现在证件照宽和高的比例为, `420px * 480px` , 如果我们使用美图秀秀修改到 `358px * 441px` 那么照片肯定是变形的, 此时如果使用 PS 就能轻松解决. 下面给出使用 PS 来修改证件照的步骤.

(1) 打开 PS , 我们新建一个 `358px * 441px` 大小的文件, 图示如下:

<img src="./images-software/image-20210208121136049.png"
    style="margin-left: 0; border-radius: 4px; width: 76%;
        box-shadow: 1px 1px 3px 2px #e5e5e5">


(2) 然后我们把图片拉入到新建的文件中,  默认新拉入的图片会成为一个处于选中状态的图层 (tip:  图层概念我不能清楚的下定义, 请自己百度或谷歌查看), 我们此时便可以按住下图中图片一圈的小方格自由编辑图层, 如果想等比例缩小/方法当前图片, (在 windows 下请按住 shift 键, macOS 中拉动每个小方格都是默认宽高等比例缩放, 请注意区别.) 编辑完毕后, 我们点击 `enter` 键即可.

<img src="./images-software/image-20210208125603191.png"
    style="margin-left: 0; border-radius: 4px; width: 76%;
        box-shadow: 1px 1px 3px 2px #e5e5e5">


(3) 最后一步为保存图片, 点击左上角的 `文件` --> `存储为 Web 所用格式`, 在当前弹框的右上部, 找到 `品质` 在其后把图片的品质设置为 50 - 60 之间, 此时点击 `存储` , 完事后查看图片应该已经小于 20kb 了.  (注意: macOS 系统的保存方式为: `文件` --> `导出` --> `存储为 Web 所用格式(旧版)`, 也是在图片的 `品质` 中设置 50 - 60 即可.)