TypeError: 'int' object has no attribute '__getitem__'

solution
from: response = proc.call(int(key_value[0]))
to: response = proc.call([int(key_value[0])])    <- should put int in []
