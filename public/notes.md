Expected output:
1. start
2. end
3. promise
4. timeout

**Explanation:** JavaScript executes synchronous code first. The Promise callback runs next because microtasks have priority over timer tasks. The `setTimeout` callback runs after the synchronous code and microtasks finish.