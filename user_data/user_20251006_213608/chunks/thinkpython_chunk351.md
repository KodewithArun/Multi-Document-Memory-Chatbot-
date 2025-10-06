1popen is deprecated now, which means we are supposed to stop using it and start using the subprocess module. But for simple cases, I ﬁnd subprocess more complicated than necessary. So I am going to keep using popen until they take it away.

14.9. Writing modules

>>> res = fp.read()

When you are done, you close the pipe like a ﬁle: >>> stat = fp.close() >>> print stat None

The return value is the ﬁnal status of the ls process; None means that it ended normally (with no errors).

For example, most Unix systems provide a command called md5sum that reads the contents of a ﬁle and computes a “checksum.” You can read about MD5 at http://en.wikipedia. org/wiki/Md5. This command provides an efﬁcient way to check whether two ﬁles have the same contents. The probability that different contents yield the same checksum is very small (that is, unlikely to happen before the universe collapses).