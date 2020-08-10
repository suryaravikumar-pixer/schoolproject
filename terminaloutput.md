# schoolproject
if you download this project you should open apps under root directory

the terminal output would be like this


Watching for file changes with StatReloader
Exception in thread django-main-thread:
Traceback (most recent call last):
  File "C:\Python\Python38\lib\threading.py", line 932, in _bootstrap_inner
    self.run()
  File "C:\Python\Python38\lib\threading.py", line 870, in run
    self._target(*self._args, **self._kwargs)
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 53, in wrapper
    fn(*args, **kwargs)
  File "C:\Python\Python38\lib\site-packages\django\core\management\commands\runserver.py", line 109, in inner_run
    autoreload.raise_last_exception()
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 76, in raise_last_exception
    raise _exception[1]
  File "C:\Python\Python38\lib\site-packages\django\core\management\__init__.py", line 357, in execute
    autoreload.check_errors(django.setup)()
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 53, in wrapper
    fn(*args, **kwargs)
  File "C:\Python\Python38\lib\site-packages\django\__init__.py", line 24, in setup  
    apps.populate(settings.INSTALLED_APPS)
  File "C:\Python\Python38\lib\site-packages\django\apps\registry.py", line 91, in populate
    app_config = AppConfig.create(entry)
  File "C:\Python\Python38\lib\site-packages\django\apps\config.py", line 90, in create
    module = import_module(entry)
  File "C:\Python\Python38\lib\importlib\__init__.py", line 127, in import_module    
    return _bootstrap._gcd_import(name[level:], package, level)
  File "<frozen importlib._bootstrap>", line 1014, in _gcd_import
  File "<frozen importlib._bootstrap>", line 991, in _find_and_load
  File "<frozen importlib._bootstrap>", line 973, in _find_and_load_unlocked
ModuleNotFoundError: No module named 'course'
Traceback (most recent call last):
  File "manage.py", line 21, in <module>
    main()
  File "manage.py", line 17, in main
    execute_from_command_line(sys.argv)
  File "C:\Python\Python38\lib\site-packages\django\core\management\__init__.py", line 401, in execute_from_command_line
    utility.execute()                                                                                                                                                   
  File "C:\Python\Python38\lib\site-packages\django\core\management\__init__.py", line 395, in execute
    self.fetch_command(subcommand).run_from_argv(self.argv)
  File "C:\Python\Python38\lib\site-packages\django\core\management\base.py", line 328, in run_from_argv
    self.execute(*args, **cmd_options)
  File "C:\Python\Python38\lib\site-packages\django\core\management\commands\runserver.py", line 60, in execute
    super().execute(*args, **options)
  File "C:\Python\Python38\lib\site-packages\django\core\management\base.py", line 369, in execute
    output = self.handle(*args, **options)
  File "C:\Python\Python38\lib\site-packages\django\core\management\commands\runserver.py", line 95, in handle
    self.run(**options)
  File "C:\Python\Python38\lib\site-packages\django\core\management\commands\runserver.py", line 102, in run
    autoreload.run_with_reloader(self.inner_run, **options)
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 599, in run_with_reloader
    start_django(reloader, main_func, *args, **kwargs)
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 584, in start_django
    reloader.run(django_main_thread)
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 299, in run
    self.run_loop()
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 305, in run_loop
    next(ticker)
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 345, in tick
    for filepath, mtime in self.snapshot_files():
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 361, in snapshot_files
    for file in self.watched_files():
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 260, in watched_files
    yield from iter_all_python_module_files()
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 105, in iter_all_python_module_files
    return iter_modules_and_files(modules, frozenset(_error_files))
  File "C:\Python\Python38\lib\site-packages\django\utils\autoreload.py", line 141, in iter_modules_and_files
  File "C:\Python\Python38\lib\pathlib.py", line 1177, in resolve
    s = self._flavour.resolve(self, strict=strict)
  File "C:\Python\Python38\lib\pathlib.py", line 200, in resolve
    return self._ext_to_normal(_getfinalpathname(s))
OSError: [WinError 123] The filename, directory name, or volume label syntax is incorrect: '<frozen importlib._bootstrap>'
