:user:`Muhtasim-Munif-Fahim` fixed :func:`iris.save` with ``compute=False``
returning a dask array, or a tuple of them, instead of the documented
:class:`~dask.delayed.Delayed`, so that ``result.compute()`` now works when
saving lazy data. (:issue:`7291`)
