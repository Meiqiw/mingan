# mingan
Dataset for  'Eﬃcient Classiﬁcation of Darknet Access Activity with Partial Traﬃc'

We uploaded the experimental data to Baidu Netdisk. link：链接：（[BaiduNetdisk](https://pan.baidu.com/s/1Wi3VQNNzTK9cObqbjee_sw)）

Extraction code：xdpt

The tree structure of the dataset is:

```
dataset_MingAn21
├── Del
│   ├── log
│   └── tcp
└── NoDel
    ├── log
    └── tcp
```

**clientdata** is the stream related to accessing website content, **clientrp** is the stream related to accessing hidden service content, and **createfast** is the stream related to downloading cached files.

For each trace, there is a txt file recording the TCP sequence in the tcp folder, and a corresponding Tor log file in the log folder with the same name. The first number of sthe filename is the type of target domain(0 for clientdata, 1 for clientrp, 2 for createfast).

For example, the following **TCP sequence file** and **Tor log file** come from the same trace, and the target domain is clientdata.

```
TCP sequence file:
0-1.txt

Tor log file:
0-1.log
```
