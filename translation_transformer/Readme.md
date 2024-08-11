# NN.Transformer와 torchtext로 언어 번역하기

따라한 자료:

- https://tutorials.pytorch.kr/beginner/translation_transformer.html

테스트 결과:

vscode에서 버전에러가 계속 발생함 -> 추후 해결 방식을 찾아봐야할거 같음

colab에서의 에러도 동일하게 발생함

에러 로그

```python
  ModuleNotFoundError                       Traceback (most recent call last)
  /usr/local/lib/python3.10/dist-packages/torchdata/datapipes/iter/util/cacheholder.py in _assert_portalocker()
      38     try:
  ---> 39         import portalocker  # noqa: F401
      40     except ImportError as e:

  ModuleNotFoundError: No module named 'portalocker'

  During handling of the above exception, another exception occurred:

  ModuleNotFoundError                       Traceback (most recent call last)
  6 frames
  /usr/local/lib/python3.10/dist-packages/torchdata/datapipes/iter/util/cacheholder.py in _assert_portalocker()
      46             raise
      47         else:
  ---> 48             raise ModuleNotFoundError(
      49                 "Package `portalocker` is required to be installed to use this datapipe."
      50                 "Please use `pip install 'portalocker>=2.0.0'` or"

  ModuleNotFoundError: Package `portalocker` is required to be installed to use this datapipe.Please use `pip install 'portalocker>=2.0.0'` or`conda install -c conda-forge 'portalocker>=2.0.0'`to install the package

  ---------------------------------------------------------------------------
  NOTE: If your import is failing due to a missing package, you can
  manually install dependencies using either !pip or !apt.

  To view examples of installing some common dependencies, click the
  "Open Examples" button below.
  ---------------------------------------------------------------------------
```
