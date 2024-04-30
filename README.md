# Simple Keylogger

This is a simple keylogger implemented in C# that logs keystrokes and emails the logs periodically.

## How it Works

The keylogger hooks into the Windows keyboard events and captures keystrokes. It maintains a buffer to store keystrokes until a certain threshold is reached, then writes them to a log file. When the log file reaches a specified length, it archives the log file, sends it via email, and clears the log file.

## Usage

1. Clone or download the repository.
2. Open the solution in Visual Studio or any compatible IDE.
3. Customize the variables in the `Program.cs` file according to your email settings and preferences.
4. Build and run the application.

## Configuration Variables

- `FROM_EMAIL_ADDRESS`: Email address used to send logs.
- `FROM_EMAIL_PASSWORD`: Password for the sending email address.
- `TO_EMAIL_ADDRESS`: Email address to receive logs.
- `LOG_FILE_NAME`: Path to the log file.
- `ARCHIVE_FILE_NAME`: Path to the archive log file.
- `INCLUDE_LOG_AS_ATTACHMENT`: Whether to include the log file as an attachment in the email.
- `MAX_LOG_LENGTH_BEFORE_SENDING_EMAIL`: Maximum length of the log file before sending it via email.
- `MAX_KEYSTROKES_BEFORE_WRITING_TO_LOG`: Maximum number of keystrokes to buffer before writing them to the log file.

## Dependencies

- `System`
- `System.Runtime.InteropServices`
- `System.Diagnostics`
- `System.Windows.Forms`
- `System.IO`
- `System.Net.Mail`
- `System.Net`

## Disclaimer

This code is provided for educational purposes only. Please use responsibly and respect privacy laws and regulations in your jurisdiction.
