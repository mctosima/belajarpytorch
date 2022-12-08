# Mempersiapkan PyTorch

Secara umum, terdapat **dua cara** untuk menjalankan PyTorch di komputer kamu, yaitu menggunakan _Jupyter Notebook Secara Online_ atau _Jupyter Notebook Secara Offline_.

## Opsi Menjalankan Notebook

### Jupyter Notebook Secara Online
Kamu dapat menggunakan beberapa layanan seperti:

- [**GoogleColab**](https://colab.research.google.com/)
- [**Kaggle**](https://www.kaggle.com/)
- [**Paperspace**](https://www.paperspace.com/)
- [Binder](https://mybinder.org/)
- [Deepnote](https://deepnote.com/)
- [SageMaker](https://aws.amazon.com/sagemaker/)
- [Azure Notebooks](https://notebooks.azure.com/)
- [CoCalc](https://cocalc.com/)

> **Catatan**: Layanan yang dicetak tebal pernah kami pergunakan dan kami rekomendasikan.

### Jupyter Notebook Secara Offline

Terdapat beberapa opsi untuk menjalankan Jupyter Notebook secara offline, yaitu:

- Menggunakan Jupyter Notebook / Jupyer Lab
- Menggunakan VSCode - [Panduan](#vscode)
- Menggunakan PyCharm
- atau Text Editor Lainnya



> **Kesimpulan**
> Jika anda seorang pemula dalam python, kami menyarankan anda menggunakan google colab karena anda tidak perlu menginstall apapun. Google colab sudah menyediakan package-package yang dibutuhkan untuk menjalankan notebook ini.

> Namun, jika anda ingin menjalankan notebook ini secara offline, kami menyarankan anda menggunakan VSCode. Cara ini juga cara terbaik apabila anda memiliki komputer dengan kartu grafis NVIDIA.

> Kami sendiri membuat bahan belajar ini dengan menjalankan Jupyter Notebook pada VSCode dengan Package Manager Conda. Terdapat package manager lain bernama pip.

## <a name="vscode"></a>Menggunakan VSCode

### Instalasi VSCode
1. Download VSCode dari [sini](https://code.visualstudio.com/download)
2. Install VSCode pada komputer kamu

### Instalasi Conda
Pada umumnya, komputer kamu sudah memiliki Python. Conda dibutuhkan agar kita dapat menginstall package yang dibutuhkan untuk menjalankan Jupyter Notebook dalam sebuah environment yang terisolasi. Jika kamu belum memiliki Conda, kamu dapat menginstallnya dengan mengikuti langkah-langkah berikut:

1. Download Installer Miniconda dari [sini](https://docs.conda.io/en/latest/miniconda.html). Sesuaikan dengan sistem operasi kamu.
2. Ikuti petunjuk instalasi yang ada [di sini](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html)
3. Install Miniconda pada komputer kamu. Kami menyarankan kamu menggunakan miniconda ketimbang anaconda. Ikuti langkah-langkah yang disediakan
4. Buka terminal (Windows) atau terminal (MacOS) dan ketikkan perintah berikut:
```bash
conda --version
```
Jika berhasil, maka akan muncul versi Conda yang terinstall

### Instalasi Ekstensi Jupyter Notebook pada VSCode
1. Buka VSCode anda
2. Pada bagian kiri, klik icon `Extensions` atau tekan `Ctrl + Shift + X` pada windows atau `Cmd + Shift + X` pada MacOS
3. Ketikkan `Jupyter` pada kolom pencarian
4. Pilih `Jupyter` dan klik tombol `Install`

atau anda dapat mengklik tautan ekstensi Jupyter Notebook pada VSCode [di sini](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

### Instalasi PyTorch, IPYKernal pada Environment Conda
- Buka terminal (Windows) atau terminal (MacOS) dan ketikkan perintah berikut:

```bash
conda create -n pytorch python=3.8
```

- Tunggu sampai proses instalasi selesai, lalu ketikkan perintah berikut:

```bash
conda activate pytorch
```

- Buka halaman PyTorch [di sini](https://pytorch.org/get-started/locally/) dan pilih opsi yang sesuai dengan sistem operasi dan hardware yang kamu gunakan. Dalam hal ini tentunya kamu memilih `package` conda dan bukan pip. Kami menyarankan kamu untuk memilih PyTorch Build Stable.

- Di bagian Compute Platform, kamu dapat memilih opsi CUDA 11.6 atau CUDA 11.7 jika kamu memiliki kartu grafis NVIDIA, atau pilih CPU jika kamu tidak memiliki kartu grafis.


> Pastikan kamu telah menginstall CUDA DRIVER dan CUDA TOOLKIT pada komputer kamu. Jika belum, kamu dapat menginstallnya dengan mengikuti langkah-langkah yang ada [di sini](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)

- Setelah itu, copy perintah yang ada di bagian `conda install` dan paste pada terminal yang sudah dibuka sebelumnya. Tunggu sampai proses instalasi selesai.

- Langkah terakhir, install IPYKernel dengan mengetikkan perintah berikut pada terminal:

```bash
conda install ipykernel
```

Selanjutnya kamu dapat membuat file baru berekstensi ipynb dan mencoba mengikuti tutorial [pengantar](./00_Pengantar.ipynb).

## Mengalami Kendala Instalasi

Anda dapat mengikuti panduan video yang ada pada tautan berikut ini:
- Instalasi conda pada Windows: [Video](https://www.youtube.com/watch?v=1mn-vA5l_90)
- Instalasi conda, vscode, jupyternotebook pada MacOS M1/m2: [Video](https://www.youtube.com/watch?v=lRJ53rPrKD0)
- Instalasi PyTorch pada M1/M2 MacOS: [Video](https://www.youtube.com/watch?v=VEDy-c5Sk8Y)
- Instalasi PyTorch dan CUDA pada Winodws: [Video](https://www.youtube.com/watch?v=GMSjDTU8Zlc)

## Masih Terkendala

Silahkan hubungi kami melalui [kolom diskusi yang ada pada github](https://github.com/mctosima/belajarpytorch/discussions). Akan ada notifikasi yang masuk ke email kontributor dan kami akan membantu kamu.