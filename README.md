# Incremental Search Traffic Dataset

The Incremental Search Traffic Dataset (**ISTD**) is a collection of 32.4k traffic samples in `pcap` format. Each sample contains network traffic captured when an English or Chinese query is typed into the search box of an incremental search website.

* English and Chinese queries are randomly selected from the [AOL search dataset](https://jeffhuang.com/search_query_logs.html) and the [THU Open Chinese Lexicon](http://thuocl.thunlp.org/) (THUOCL), respectively.
* Each language contains 1.8k queries with lengths ranging from 10 to 40 characters (60 queries per length).
* Websites include Google, Tmall, Facebook, Baidu, Yahoo, Wikipedia, Csdn, Twitch, and Bing (9 in total).
* User's typing rhythm is simulated using the timing model trained on the [136M keystroke dataset](https://userinterfaces.aalto.fi/136Mkeystrokes/).

The traffic capture process ran from September 23 to October 4, 2020, lasted about 12 days.

***Note:*** This dataset is for NON-COMMERCIAL RESEARCH USE ONLY.

## Content
ISTD consists of two parts:
* query/
  * AOL/
    * lxx_n60.csv: list of 60 English queries with a length of (xx) characters.
  * THUOCL/
    * lxx_n60.csv: list of 60 Chinese queries with a Pinyin syllable length of (xx) characters.
	
* pcap/yy/
  * AOL/
  * THUOCL/
    * lxx_n60/zz.pcap: traffic sample captured while typing query (zz) in website (yy).

## Getting the dataset
The dataset is available here:
* [ISTD](https://mega.nz/file/0I4SQCjJ#Wzqp1v7XvnBzhn3jcCC2hcQdcT3k6jzzOmxBvAhOnTc) (10.15 GB, SHA1: C3089F76E952A8218881B6D8A11E214CF091604E)

## Related repository
* [QAIS](https://github.com/ld258166011/QAIS): the data collection tool that captures network traffic while a query is typed into an incremental search website.
