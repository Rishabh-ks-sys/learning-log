# Learning Log - Tools Registry

## 1. Date & Tools
•⁠  ⁠*Date:* October 21, 2026
•⁠  ⁠*Tools Met:* ⁠ ffmpeg ⁠ and ⁠ qrencode ⁠

## 2. Tool Purposes
•⁠  ⁠*ffmpeg:* A multimedia framework used to convert, record, and stream digital audio and video files.
•⁠  ⁠*qrencode:* A command-line utility that takes input text or URLs and formats them into a scannable QR code image.

## 3. Successful Commands
•⁠  ⁠*ffmpeg command:*
  ⁠ bash
  ffmpeg -i input.mp4 -vf "fps=10,scale=320:-1:flags=lanczos" output.gif
   ⁠
•⁠  ⁠*qrencode command (Text):*
  ⁠ bash
  qrencode -o hello.png "We will return in Avengers: Doomsday"
   ⁠
•⁠  ⁠*qrencode command (URL):*
  ⁠ bash
  qrencode -o repo.png "https://github.com"
   ⁠

## 4. Troubleshooting (What Broke & How it Was Fixed)
1.⁠ ⁠*Error:* ⁠ ffmpeg ⁠ command failed because the output path or filename was missing.
   * *Fix:* Checked the syntax to ensure both the input flag ⁠ -i ⁠ and a final destination filename (e.g., ⁠ output.gif ⁠) were explicitly provided.
2.⁠ ⁠*Error:* Special characters or colons in the URL caused the terminal shell to misinterpret the command.
   * *Fix:* Wrapped the entire URL string inside straight quotation marks (⁠ "https://..." ⁠) to protect the string from shell expansion.

## 5. The Five Steps for Documenting Tools
1.⁠ ⁠*What is it for?* Define its core purpose in one sentence.
2.⁠ ⁠*Find the shape.* Check documentation (⁠ man ⁠ pages or ⁠ --help ⁠) to understand basic configuration.
3.⁠ ⁠*Smallest thing that works.* Run the bare minimum working example command.
4.⁠ ⁠*Change one thing.* Modify an option or parameter (like input text or file source) to verify behavior.
5.⁠ ⁠*Break it on purpose.* Intentionally cause an error to recognize diagnostic outputs and limitations.

## 6. Next Steps / Things to Try
•⁠  ⁠Find out how to change the foreground and background pixel colors of generated QR codes using ⁠ qrencode ⁠ flags.
*
