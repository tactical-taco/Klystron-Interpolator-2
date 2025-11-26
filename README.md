🛠️ Klystron Cavity Interpolator

A simple desktop application built on Windows Forms (WinForms) for calculating the optimal tuning cavity settings for a Klystron tube using linear interpolation between two known calibration points.

✨ Features

    Linear Interpolation: Calculates 6 interpolated cavity settings (C1 through C6) based on two input calibration frequencies and a target Transmit Frequency.

    Structured Export: Exports the complete calibration data (Lower, Upper, and Interpolated settings) to a clean, formatted HTML report for easy record-keeping and sharing.

    Printing Support: Provides a Print Preview and printing functionality for generating hard copies of the structured report.

    Fixed Interface: The window is non-resizable, ensuring a consistent layout and user experience.

    User Assistance: Includes simple Usage and About menu items for quick reference on operation and version information.

🚀 How to Use

The application follows a simple process to determine the optimal tuning settings.

    Input Calibration Data:

        Enter the Lower Frequency (FL​) and its corresponding cavity settings into the C1L through C6L columns.

        Enter the Upper Frequency (FU​) and its corresponding cavity settings into the C1U through C6U columns.

        Enter the desired Transmit Frequency (FXMT​) into the designated input box.

    Calculate Settings:

        Navigate to the Actions menu and select Interpolate.

        The calculated optimal settings will appear in the C1-C6 (Output) column, rounded to one decimal place.

    Save or Print Report:

        To Export: Go to File > Export Results... to save the clean HTML report file.

        To Print: Go to File > Print... to view the Print Preview and print the structured report.

⚙️ Technical Details

Interpolation Formula

The core of the application uses the standard linear interpolation formula applied independently to each of the six cavity settings (S):
SX​=SL​+(FXMT​−FL​)⋅FU​−FL​SU​−SL​​

Where:

    SX​ = Interpolated Cavity Setting (Output)

    SL​ = Lower Cavity Setting (Input)

    SU​ = Upper Cavity Setting (Input)

    FXMT​ = Transmit Frequency (Target)

    FL​ = Lower Frequency (Input)

    FU​ = Upper Frequency (Input)

Project Stack

    Framework: .NET (Windows Forms)

    Language: C#
