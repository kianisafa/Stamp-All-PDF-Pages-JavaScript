
# 📄 PDF Stamping Guide

Welcome to the **PDF Stamping Guide**! This document provides a comprehensive overview of how to apply, customize, and manage stamps in your PDF documents using Adobe Acrobat. Whether you're a novice or a seasoned pro, this guide will help you master the art of PDF stamping. 

## 📋 Table of Contents

- [Introduction](#introduction)
- [Stamp Tool Categories](#stamp-tool-categories)
- [Opening the Stamps Palette](#opening-the-stamps-palette)
- [Applying a Stamp](#applying-a-stamp)
- [Changing a Stamp’s Location or Appearance](#changing-a-stamps-location-or-appearance)
- [Moving a Stamp to the Favorites List](#moving-a-stamp-to-the-favorites-list)
- [Creating a Custom Stamp](#creating-a-custom-stamp)
- [Editing a Custom Stamp](#editing-a-custom-stamp)
- [Deleting a Custom Stamp](#deleting-a-custom-stamp)
- [Deleting a Custom Stamp Category](#deleting-a-custom-stamp-category)
- [JavaScript Code for Stamping Across Multiple Pages](#javascript-code-for-stamping-across-multiple-pages)
- [Developer](#developer)
- [Note](#note)
- [Contact](#contact)

## 📝 Introduction

Stamps in Adobe Acrobat work like rubber stamps on paper documents. You can choose from predefined stamps or create your own. Dynamic stamps pull information from your computer and preferences, displaying name, date, and time on the stamp.

## 📚 Stamp Tool Categories

1. **Dynamic Stamp** 🕒
2. **Sign Here Stamp** ✍️
3. **Standard Business Stamp** 📈
4. **Custom Stamp** 🛠️

## 🗂️ Opening the Stamps Palette

To open the Stamps Palette, you can:
- Navigate to `Tools` > `Stamp` > `Stamps Palette`.
- Or go to `Tools` > `Comment` > `Stamps` > `Show Stamps Palette`.

## 🖊️ Applying a Stamp

1. Click the **Stamp tool**. The most recently used stamp is selected.
2. In the **Stamps Palette**, choose a category and select a stamp.
3. Click on the document page where you want the stamp or drag a rectangle to define its size and placement.
4. If prompted, enter your identity information in the **Identity Setup** dialog box.

## 🔄 Changing a Stamp’s Location or Appearance

Using the **Select tool** or the **Hand tool**:
- **Move**: Drag the stamp to a new location.
- **Resize**: Click and drag a corner handle.
- **Rotate**: Click, move the pointer over the handle at the top, and drag when the rotate icon appears.
- **Delete**: Right-click and choose **Delete**.
- **Opacity/Color**: Right-click and choose **Properties**. Adjust settings in the **Appearance** tab.

## ⭐ Moving a Stamp to the Favorites List

1. Using the **Select tool** or the **Hand tool**, select the stamp on the page.
2. In the secondary toolbar of the **Comment tool**, click the **Stamp tool** and choose **Add Current Stamp To Favorites**.

## 🛠️ Creating a Custom Stamp

1. Open the **Stamps Palette**:
   - `Tools` > `Stamp` > `Stamps Palette`
   - `Tools` > `Comment` > `Stamps` > `Show Stamps Palette`
2. Click **Import** and select the file (PDF, JPEG, bitmap, AI, PSD, DWT, DWG).
3. Choose a category or type a new one, name the custom stamp, and click **OK**.

## ✏️ Editing a Custom Stamp

1. Open the **Stamps Palette**:
   - `Tools` > `Stamp` > `Stamps Palette`
   - `Tools` > `Comment` > `Stamps` > `Show Stamps Palette`
2. Choose the stamp category, right-click the stamp, and select **Edit**.
3. Edit the category or name of the stamp, or replace the image, and click **OK**.

## 🗑️ Deleting a Custom Stamp

1. Open the **Stamps Palette**:
   - `Tools` > `Stamp` > `Stamps Palette`
   - `Tools` > `Comment` > `Stamps` > `Show Stamps Palette`
2. Choose the stamp category, right-click the custom stamp, and choose **Delete**.

## 🚮 Deleting a Custom Stamp Category

1. Choose `Tools` > `Stamp` > `Custom Stamps`.
2. Or choose `Tools` > `Comment` > `Stamps` > `Custom Stamps` > `Manage Stamps`.
3. Select the category you want to delete and click **Delete**.

## 🔧 JavaScript Code for Stamping Across Multiple Pages

Use the following JavaScript code to stamp across multiple pages:

```javascript
this.syncAnnotScan();
var annt = this.getAnnots(this.pageNum)[0];
var props = annt.getProps();
for (var i = 0; i < this.numPages; i++) {
  props.page = i;
  if (i != this.pageNum) this.addAnnot(props);
}
```

## 👨‍💻 Developer
This guide and the associated code were developed by **Safa Kiani**. 💼

## 📝 Note
This code has been tested only with **Adobe Acrobat**. ⚙️

## 📬 Contact
If you have any questions or need further information, please feel free to reach out:

- **GitHub**: [kianisafa](https://github.com/kianisafa)
- **Email**: kianisafaa@gmail.com
- **Telegram**: [kianisafa](https://t.me/+12363343330)
- **Instagram**: [kianisafa](https://www.instagram.com/kianisafa/)


Thank you for using this guide! 😊
