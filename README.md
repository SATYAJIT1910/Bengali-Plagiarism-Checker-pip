# Bengali Plagiarism Checker

Introducing a Python library for detecting plagiarism in Bengali texts. This library comprises 200 Bengali books with approximately 4100 pages sourced from the National Digital Library, processed using the Tesseract OCR engine. With just two lines of code, you can check for similarities in Bengali written content. If a high degree of similarity is found, it will display the book title, author name, and other details. You can install the library using the following command in the terminal: 
```
pip install BengaliPlagiarismChecker
```


<hr>
<br>

## Sample Usage

```
import BengaliPlagiarismChecker as bpc #importing package

#input text
text="""

বসন্তাগমে কামিনী রায় বসন্ত কি সহসা এ নির্জন আবাসে পশিয়াছ চুপি চুপি? নবীন পল্পবে
সাজিয়াছে তরুরাজি। ঝেড়ে দিলে কবে পুরাতন জীর্ণপত্র শীতল বাতাসে বাতাবি ফুলের গন্ধ ধীরে ধীরে ভেসে আসে আমার গবাক্ষপথে ঘন কুহুরবে মুখরিত আম্রবন বসন্তই হবে উদ্যান উজ্জল শত শ্বেত পুস্প হাসে আজিও ধরনি মরে রেখেছে ধরিয়া তার স্বর্ণ কারাগারে বর্ণ গন্ধ গানে রসে স্পর্শে দিতে চাহে দেহে আর চিতে নব প্রাণ, কিন্তু হায় নিঃশেষে ভরিয়া কই দিতে পারে, মধু? দূরে কোন্খানে থাকে অদেহীরা, বধু, পারো বলে দিতে?

"""
#method to find out plagiarism
bpc.check(text)

'''
OUTPUT

[[194, #BookID
  'State Council of Educational Research and Training (SCERT)', #Author or Publisher
  'সাহিত্য মালঞ্চ', #Book name
  14,  # Page number
  23.88]] #Similarity Score


'''

```
<hr>
<br>
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
