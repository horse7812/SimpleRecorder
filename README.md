SimpleRecorder
==============

* camera.c:      基于v4l2的摄像头采集,支持一般的摄像头
* textoverlay.c: 在图片上叠加ASCII字符,目前做得比较简陋
* preview.c:     往framebuffer写图像,实现预览
* encoder.c:     H264编码器
* output.c:      把编码后的H264码流写入MKV容器
* main.c:        主函数,调用以上代码中的接口

* 未编码图像用picture_t传递,内部是I420格式,编码后的码流用encoded_pic_t传递

---
