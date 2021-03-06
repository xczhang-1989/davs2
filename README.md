# davs2

**davs2** is an open-source decoder of `AVS2/IEEE1857.4` video coding standard.

[![GitHub tag](https://img.shields.io/github/tag/pkuvcl/davs2.svg?style=plastic)]()
[![GitHub issues](https://img.shields.io/github/issues/pkuvcl/davs2.svg)](https://github.com/pkuvcl/davs2/issues)
[![GitHub forks](https://img.shields.io/github/forks/pkuvcl/davs2.svg)](https://github.com/pkuvcl/davs2/network)
[![GitHub stars](https://img.shields.io/github/stars/pkuvcl/davs2.svg)](https://github.com/pkuvcl/davs2/stargazers)

## Compile it
### Windows
Use VS2013 or latest version of  visual studio open the `./build/vs2013/davs2.sln` solution and set the `davs2` as the start project.

#### Notes
1. A `shell executor`, i.e. the bash in git for windows, is needed and should be found in `PATH` variable.
 For example, the path `C:\Program Files\Git\bin` can be added if git-for-windows is installed.
2. `vsyasm` is needed and `1.2.0` is suggested for windows platform. It can be downloaded through: http://yasm.tortall.net/Download.html .
 A later version `1.3.0`, can be found in https://github.com/luofalei/yasm/tree/vs2013 .

### Linux
```
$ cd build/linux
$ ./configure
$ make
```

## Try it

```
./davs2 -i test.avs -o test_dec.yuv [-r test_rec.yuv -t N]
```

### Parameter Instructions
| Parametesr       |   Alias     |   Result  |
| :--------:       | :---------: | :--------------: |
| --input=test.avs | -i test.avs |  Setting the input bitstream file |
| --output=dec.yuv | -o dec.yuv  |  Setting the output YUV file |
| --psnr=rec.yuv   | -r rec.yuv  |  Setting the reference reconstruction YUV file |
| --threads=N      | -t N        |  Setting the threads for decoding (default: 1) |
| --verbose        | -v          |  Enable decoding status every frame (Default: Enabled) |
| --help           | -h          |  Showing this instruction |

## Homepages

[PKU-VCL][1]

[git repository on Gitee.com][2]

[git repository on Github.com][3]

  [1]: http://vcl.idm.pku.edu.cn/ "PKU-VCL"
  [2]: https://gitee.com/pkuvcl/davs2 "gitee repository"
  [3]: https://github.com/pkuvcl/davs2 "github repository"