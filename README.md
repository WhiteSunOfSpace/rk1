#first control work

#analysis of github sourse

1.  git clone https://github.com/facebook/folly
    find . -type f | wc -l
    ```shell
    2281
    ```

2.  find . -type f -exec du -h {} + >'/home/vboxuser/WhiteSunOfSpace/workspace/rk/3.txt'
    ```shell
    answer is in the file 3.txt in repository
    ```

3.  cloc /home/vboxuser/WhiteSunOfSpace/workspace/folly
    ```shell
    2251 text files.
    2249 unique files.                                          
    105 files ignored.

    github.com/AlDanial/cloc v 1.90  T=3.03 s (709.9 files/s, 197069.2 lines/s)
    -----------------------------------------------------------------------------------
    Language                         files          blank        comment           code
    -----------------------------------------------------------------------------------
    C++                               1022          42531          38734         244133
    C/C++ Header                       944          30799          73020         137673
    Python                              40           1983           2165           8395
    Markdown                            46           1854              0           6216
    CMake                               45            541           1380           3872
    Cython                              26            216            394            786
    YAML                                 7             13             16            501
    Assembly                             2             83            111            343
    Bourne Shell                         7             69            124            326
    diff                                 3             10             39            117
    C                                    2             23             61             86
    Ruby                                 1             13             26             73
    DOS Batch                            1              2              0             24
    make                                 1             10              1             22
    CSS                                  1              1             15              7
    Verilog-SystemVerilog                1              0              1              3
    SVG                                  1              0              0              1
    -----------------------------------------------------------------------------------
    SUM:                              2150          78148         116087         402578
    -----------------------------------------------------------------------------------
    ```

4.  find . -type f -name "*.clang-format" | wc -l
    ```shell
     2
    ```

5.  [ ! -d "/src/" ] && echo "no such directory"
    ```shell
    no such directory
    ```

6.  find . -type f  -iname "*socket*" | wc -l
    ```shell
    73
    ```

7.  find . -type f  -iname "*select*" | wc -l
    ```shell
    3
    ```

8.  find /home/vboxuser/WhiteSunOfSpace/workspace/folly -type f -exec grep -iEo 'microsoft|google|intel' {} + | wc -l
    ```shell
    grep: /home/vboxuser/WhiteSunOfSpace/workspace/folly/.git/index: binary file matches
    319
    ```

9.  find $(pwd) -name "LICENSE*"
    ```shell
    /home/vboxuser/WhiteSunOfSpace/workspace/folly/build/fbcode_builder/LICENSE
    /home/vboxuser/WhiteSunOfSpace/workspace/folly/LICENSE
    ```

10. grep -iE 'BSD|GNU|MIT|APSL|Apache|GPL|AGPL|LGPL' /home/vboxuser/WhiteSunOfSpace/workspace/folly/LI
    ```shell
                                Apache License
                        http://www.apache.org/licenses/
      including but not limited to software source code, documentation
      not limited to compiled object code, generated documentation,
      submitted to Licensor for inclusion in the Work by the copyright owner
      or by an individual or Legal Entity authorized to submit on behalf of
      the copyright owner. For the purposes of this definition, "submitted"
      to the Licensor or its representatives, including but not limited to
      with the Work to which such Contribution(s) was submitted. If You
      any Contribution intentionally submitted for inclusion in the Work
      implied, including, without limitation, any warranties or conditions
      Limitation of Liability. In no event and under no legal theory,
      Work (including but not limited to damages for loss of goodwill,
      in the Software without restriction, including without limitation the rights
      copies of the Software, and to permit persons to whom the Software is
      IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    ```
