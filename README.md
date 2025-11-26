🛠️ Klystron Cavity Interpolator

A simple, fixed-size desktop application built on Windows Forms (WinForms) for calculating the optimal tuning cavity settings for a Klystron tube using linear interpolation between two known calibration points.

✨ Features

Linear Interpolation: Calculates 6 interpolated cavity settings (C1 through C6) based on two input calibration frequencies and a target Transmit Frequency.

Structured Export: Exports the complete calibration data (Lower, Upper, and Interpolated settings) to a formatted HTML report for easy record-keeping and readability.

Printing Support: Provides a Print Preview and printing functionality for generating hard copies of the tuning report.

User Assistance: Includes simple Usage and About menu items for quick reference on operation and version information.

Fixed Interface: The window is non-resizable (FixedSingle border style) to maintain a consistent user experience and layout.

🚀 How to Use

The application follows a simple three-step process:

Input Calibration Data:

Enter the Lower Frequency (F1) and its corresponding cavity settings into the C1L through C6L columns.

Enter the Upper Frequency (F2) and its corresponding cavity settings into the C1U through C6U columns.

Enter the desired Transmit Frequency (F_XMT) into the designated input box.

Calculate Settings:

Navigate to the Actions menu and select Interpolate.

The calculated optimal settings for the Transmit Frequency will appear in the C1-C6 (Output) column, rounded to one decimal place.

Save or Print Report:

To Export: Go to File > Export Results... to save a clean HTML report file.

To Print: Go to File > Print... to view the Print Preview and print the structured report.

⚙️ Technical Details

Project Stack

Framework: .NET (or .NET Framework, depending on the version used)

Application Type: Windows Forms (WinForms)

Language: C#

Interpolation Formula

The application uses the standard linear interpolation formula for each cavity setting (S_x):

$$S_{X} = S_{L} + (F_{XMT} - F_{L}) \cdot \frac{S_{U} - S_{L}}{F_{U} - F_{L}}$$

Where:

$S_X$ = Interpolated Cavity Setting

$S_L$ = Lower Cavity Setting

$S_U$ = Upper Cavity Setting

$F_{XMT}$ = Transmit Frequency

$F_L$ = Lower Frequency

$F_U$ = Upper Frequency
