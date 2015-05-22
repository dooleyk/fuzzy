# fuzzy language

Language extension created using...

Project -> New Project from Template and select the Create Komodo Language
 
Did not check 'code intelligence facilities' wizard option.

Get langinfo error popping up repeatedly in 9.0 when editing a fuzzy (.fzy) file, though color coding and Edit Preferences Language stuff works. (This same error also occurs in 8.0 though it is less noticable because it only shows up in the log, and not in popup boxes.)

[2015-05-22 07:49:08,524] [ERROR] codeintel.langintel: error getting langinfo for 'Fuzzy'
Traceback (most recent call last):
  File "/home/dooleyk/Komodo-IDE-9/lib/mozilla/python/komodo/codeintel2/langintel.py", line 61, in langinfo
    self._langinfo_cache = self.mgr.lidb.langinfo_from_komodo_lang(self.lang)
  File "/home/dooleyk/Komodo-IDE-9/lib/mozilla/python/komodo/langinfo.py", line 311, in langinfo_from_komodo_lang
    raise LangInfoError("no info on %r komodo lang" % komodo_lang)
LangInfoError: no info on u'Fuzzy' komodo lang

