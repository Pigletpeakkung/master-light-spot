Code with syntax highlighting
Here’s some code with syntax highlighting:

-- | Inefficient quicksort in haskell.
qsort :: (Enum a) => [a] -> [a]
qsort []     = []
qsort (x:xs) = qsort (filter (< x) xs) ++ [x] ++
               qsort (filter (>= x) xs) 
Try changing the highlighting style to see what effect this has.

Here’s some python, with numbered lines:

class FSM(object):

"""This is a Finite State Machine (FSM).
"""

def __init__(self, initial_state, memory=None):

    """This creates the FSM. You set the initial state here. The "memory"
    attribute is any object that you want to pass along to the action
    functions. It is not used by the FSM. For parsing you would typically
    pass a list to be used as a stack. """

    # Map (input_symbol, current_state) --> (action, next_state).
    self.state_transitions = {}
    # Map (current_state) --> (action, next_state).
    self.state_transitions_any = {}
    self.default_transition = None
    ...
