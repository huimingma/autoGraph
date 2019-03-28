 //因为没有后台接口，数据都存储在本地的，storage中signImage就是签名的图片
 
 //js
 onLoad: function (options) {
    this.handwriting = new Handwriting(this, {
      lineColor: this.data.lineColor,
      slideValue: this.data.slideValue,
    })
  },

  // 初始化需传入两个参数 
  // lineColor  字体颜色 默认#1A1A1A 
  // slideValue 字体粗细 默认50（内置 0，25，50, 75, 100 5档粗细）

  /**
   *   example:
   *   this.handwriting = new Handwriting(this, {
        lineColor: '#1A1A1A',
        slideValue: 50,
      })
   */
   
   // 两个内置函数
   this.handwriting.selectColorEvent(color);   // 传入颜色参数 改变字体颜色
   this.handwriting.selectSlideValue(slideValue);  // 传入粗细参数 0,25,50,75,100 改变字体粗细


