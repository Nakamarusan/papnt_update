cope with this problem

Traceback (most recent call last):
  File "/usr/local/bin/papnt", line 8, in <module>
    sys.exit(main())
  File "/usr/local/lib/python3.10/dist-packages/click/core.py", line 1157, in __call__
    return self.main(*args, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/click/core.py", line 1078, in main
    rv = self.invoke(ctx)
  File "/usr/local/lib/python3.10/dist-packages/click/core.py", line 1688, in invoke
    return _process_result(sub_ctx.command.invoke(sub_ctx))
  File "/usr/local/lib/python3.10/dist-packages/click/core.py", line 1434, in invoke
    return ctx.invoke(self.callback, **ctx.params)
  File "/usr/local/lib/python3.10/dist-packages/click/core.py", line 783, in invoke
    return __callback(*args, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/papnt/cli.py", line 56, in doi
    update_unchecked_records_from_doi(database, config['propnames'])
  File "/usr/local/lib/python3.10/dist-packages/papnt/mainfunc.py", line 48, in update_unchecked_records_from_doi
    _update_record_from_doi(database, doi, record['id'], propnames)
  File "/usr/local/lib/python3.10/dist-packages/papnt/mainfunc.py", line 32, in _update_record_from_doi
    prop = prop_maker.from_doi(doi, propnames)
  File "/usr/local/lib/python3.10/dist-packages/papnt/notionprop.py", line 62, in from_doi
    return self._make_properties(doi_style_info, propnames)
  File "/usr/local/lib/python3.10/dist-packages/papnt/notionprop.py", line 118, in _make_properties
    authors = self._make_author_list(info['author'])
  File "/usr/local/lib/python3.10/dist-packages/papnt/notionprop.py", line 152, in _make_author_list
    authors_.append(author['family'].replace(' ', '_'))
KeyError: 'family'
