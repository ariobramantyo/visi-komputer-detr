# Face Detection Using Detection Transformer

## Step 1.
Download [WiderFace dataset](http://shuoyang1213.me/WIDERFACE/) kemudian unzip file dan masukkan ke dalam dataset folder

## Step 2.
Pindahkan direktori ke folder dataset dan jalankan perintah berikut untuk mengubah dataset WiderFace menjadi COCO format
```
$ python face_to_coco.py
```

## Step 3.
Pindahkan direktori ke folder detr dan run main.py
```
$ python main.py --dataset_file face --data_path ../dataset/ --output_dir output
```

## Step 4.
Run test.py
```
$ python test.py --data_path ../dataset/WIDER_test/images/ --resume [path_to_checkpoint.pth]
```

Hasil training model dapat didownload [di sini](https://drive.google.com/drive/folders/1KtuyzGpqrB8FiODTRwF5A-5L42QX9ALm?usp=sharing)
