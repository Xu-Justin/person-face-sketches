# [Person Face Sketches](https://www.kaggle.com/datasets/almightyj/person-face-sketches)

[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Xu-Justin/person-face-sketches) [![Kaggle](https://img.shields.io/badge/Kaggle-035a7d?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/almightyj/person-face-sketches)

<table>
  <tr>
    <td><img src="resources/photos/0.jpg"></td>
    <td><img src="resources/photos/1.jpg"></td>
    <td><img src="resources/photos/3.jpg"></td>
    <td><img src="resources/photos/4.jpg"></td>
    <td><img src="resources/photos/5.jpg"></td>
  </tr>
  <tr>
    <td><img src="resources/sketches/0.jpg"></td>
    <td><img src="resources/sketches/1.jpg"></td>
    <td><img src="resources/sketches/3.jpg"></td>
    <td><img src="resources/sketches/4.jpg"></td>
    <td><img src="resources/sketches/5.jpg"></td>
  </tr>
</table>

## About Dataset

Images were taken from the [CelebAMask-HQ](https://github.com/switchablenorms/CelebAMask-HQ) dataset without `Eyeglasses`, `Wearing_Hat` attributes, and `Yaw`, `Pitch`, `Raw` absolute degrees equal or less than 20.

Then theses images were filtered with `ImageFilter.FIND_EDGES`, `ImageFilter.BLUR`, `ImageFilter.SHARPEN`, `ImageOps.invert()` and `ImageEnhance.Contrast().enhance(1.5)` sequentially to produce rought sketches. Furthermore, theses rought skecthes are simplified using [Sketch Simplification](https://esslab.jp/~ess/research/sketch/).

---

This project was developed as part of Nodeflux Internship x Kampus Merdeka.