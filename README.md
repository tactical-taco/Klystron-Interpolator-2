# 🛠️ Klystron Cavity Interpolator

A simple desktop application built on Windows Forms (WinForms) for calculating the optimal tuning cavity settings for a Klystron tube using linear interpolation between two known calibration points.

## ✨ Features

* **Linear Interpolation:** Calculates 6 interpolated cavity settings (C1 through C6) based on two input calibration frequencies and a target Transmit Frequency.
* **Structured Export:** Exports the complete calibration data (Lower, Upper, and Interpolated settings) to a clean, formatted **HTML report** for easy record-keeping and sharing.
* **Printing Support:** Provides a **Print Preview** and printing functionality for generating hard copies of the structured report.
* **Fixed Interface:** The window is non-resizable, ensuring a consistent layout and user experience.
* **User Assistance:** Includes simple **Usage** and **About** menu items for quick reference on operation and version information.

## 🚀 How to Use

The application follows a simple process to determine the optimal tuning settings.

1.  **Input Calibration Data:**
    * Enter the **Lower Frequency** ($F_L$) and its corresponding cavity settings into the **C1L** through **C6L** columns.
    * Enter the **Upper Frequency** ($F_U$) and its corresponding cavity settings into the **C1U** through **C6U** columns.
    * Enter the desired **Transmit Frequency** ($F_{XMT}$) into the designated input box.

2.  **Calculate Settings:**
    * Navigate to the **Actions** menu and select **Interpolate**.
    * The calculated optimal settings will appear in the **C1-C6** (Output) column, rounded to one decimal place.

3.  **Save or Print Report:**
    * **To Export:** Go to **File** > **Export Results...** to save the clean HTML report file.
    * **To Print:** Go to **File** > **Print...** to view the Print Preview and print the structured report.

## ⚙️ Technical Details

### Interpolation Formula

The core of the application uses the standard linear interpolation formula applied independently to each of the six cavity settings ($S$):

$$S_{X} = S_{L} + (F_{XMT} - F_{L}) \cdot \frac{S_{U} - S_{L}}{F_{U} - F_{L}}$$

Where:
* $S_X$ = Interpolated Cavity Setting (Output)
* $S_L$ = Lower Cavity Setting (Input)
* $S_U$ = Upper Cavity Setting (Input)
* $F_{XMT}$ = Transmit Frequency (Target)
* $F_L$ = Lower Frequency (Input)
* $F_U$ = Upper Frequency (Input)


[Image of linear interpolation calculation graph]


### Project Stack

* **Framework:** .NET (Windows Forms)
* **Language:** C#

-----

## 🤝 Contribution

Feel free to open issues for bugs or suggest new features\!

-----

### 💖 Support the Project
This app is a passion project built in my spare time. If you find the **ASOS Monitor** useful and want to show your appreciation, you can literally [buy me a coffee](https://buymeacoffee.com/ke5wydf)! Your support helps keep me fueled for bug fixes and new features.

[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-orange?style=flat&logo=buy-me-a-coffee)](https://buymeacoffee.com/ke5wydf)
