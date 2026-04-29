1. values added: 20
2. final result: 20
3. You should avoid var because it is function-scoped as opposed to block-scoped. This means that if its used and should only be accessed in an if block or loop, it will still be accessible outside of that block. It can cause numerous issues like naming conflicts, value/assignment conflicts, and other unexpected bugs.
4. values added: 20
5. ReferenceError: result is not defined. Since variables declared with let are block-scoped, they only exist in the block they are defined in. That means that when the code exists the block, the result variable no longer exists, so trying to access result is not possible and returns an error.
6. At line 9, there is an error because variables declared using const can't be reassigned and attempting to do so will cause an error. So the code will return an error at line 7 when there is an attempt to reassign result.
7. The code will crash at line 7 due to reassignment, but even if it was fixed, const is block-scoped and like let only exists in the block so exiting means that variable no longer exists.