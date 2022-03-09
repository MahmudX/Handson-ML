# Save Strategy

Use dill to save and  restore `.ipynb` session variables.

```py
try:
    !pip install dill
except:
    pass
try:
    import dill
    dill.load_session('notebook_env.db')
except:
    pass

try:
    import dill
    dill.dump_session('notebook_env.db')
except:
    pass
```