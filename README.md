
```
def summary(text, key, max_word, max_sent):
    """
    Parameters
    ----------
    text: string, unicode
    key: string, unicode
    max_word: int
    max_sent: int

    Returns:
    --------
    sentence_list: array of string
    """
    summ = Summarization({"text": text,
                          "key": key,
                          "max_sent": max_sent,
                          "max_word": max_word
                          })
    return summ.get_summary()
```


summary(u"年终钜惠！锐志最高优惠2.5万元   2014年01月21日，
大连华通丰田锐志最高优惠2.5万元，感兴趣的朋友可以到店咨询购买，具体优惠信息如下：      锐志",
u"丰田", 1, 150)
