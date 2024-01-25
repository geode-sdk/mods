# Fast Format

This mod optimizes\* the function `CCString::initWithFormatAndValist`, which is used in quite a lot of places by rob (via `CCString::createWithFormat`).

The original code looks like this:
```cpp
#define kMaxStringLen (1024 * 100)

bool CCString::initWithFormatAndValist(const char* format, va_list ap)
{
    bool bRet = false;
    char* pBuf = (char*)malloc(kMaxStringLen);
    if (pBuf != NULL)
    {
        vsnprintf(pBuf, kMaxStringLen, format, ap);
        m_sString = pBuf;
        free(pBuf);
        bRet = true;
    }
    return bRet;
}
```

This means that each time this function is called, 100KiB is allocated and then quickly deallocated. This is quite silly and could result in poor perfomance.

\* It is unsure whether this mod actually helps perfomance in any way.