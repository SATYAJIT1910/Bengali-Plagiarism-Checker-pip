# Bengali Plagiarism Checker

Bengali Plagiarism Checker library contains database of 200 books with over 4100 pages in it for detection of plagiarism in Bengali texts. This library is based on a paper titled "Plagiarism Detection in the Bengali Language: A Text Similarity-Based Approach".
<br>
<b>Cite the paper as :</b><br>
```
@misc{https://doi.org/10.48550/arxiv.2203.13430,
  doi = {10.48550/ARXIV.2203.13430},
  
  url = {https://arxiv.org/abs/2203.13430},
  
  author = {Ghosh, Satyajit and Ghosh, Aniruddha and Ghosh, Bittaswer and Roy, Abhishek},
  
  keywords = {Computation and Language (cs.CL), FOS: Computer and information sciences, FOS: Computer and information sciences},
  
  title = {Plagiarism Detection in the Bengali Language: A Text Similarity-Based Approach},
  
  publisher = {arXiv},
  
  year = {2022},
  
  copyright = {Creative Commons Attribution 4.0 International}
}
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
