# Audio Format Conversion Script
A recursive audio transcoder

Overview
The audio_format_conversion.sh script is a Bash script designed to convert audio files from various formats (FLAC, ALAC, WAV) to user-specified formats (MP3, Opus, Ogg). The script uses the ffmpeg tool to perform the conversions and allows customization of parameters such as quality, bitrate, and compression level.

Features
Format Support: Converts FLAC, ALAC, and WAV files to MP3, Opus, or Ogg formats.

Quality Control: Allows users to specify quality settings (0-9) for MP3 and Ogg formats.

Opus Configuration: For Opus format, users can set bitrate (64k-256k) and compression level (0-10).

Directory Handling: Supports batch conversion of audio files in a specified input directory and organizes the output in a user-defined directory structure.

Usage
Run the Script:

Save the script to a file, e.g., audio_format_conversion.sh.
Make it executable: chmod +x audio_format_conversion.sh.
Run the script: ./audio_format_conversion.sh.

Enter Conversion Settings:

Choose the desired audio format (mp3, opus, ogg).
Enter quality, bitrate, or compression level based on the selected format.

Specify Directories:

Enter the input directory containing audio files to be converted.
Enter the output directory where converted files will be saved.

Conversion Process:

The script will create the output directory if it doesn't exist.
It will find audio files in the input directory, convert them according to the specified format, and save them in the output directory.
Example

$ ./audio_format_conversion.sh
Enter the desired audio format (mp3, opus, ogg): mp3
Enter the desired quality (0-9): 5
Enter the input directory: /path/to/input
Enter the output directory: /path/to/output
Notes
Ensure you have ffmpeg installed on your system.
The script supports FLAC, ALAC, and WAV input formats.
