Add your answers to the Algorithms exercises here.

I.
    a. O(1)
    b. O(logn)
    c. O(logn)
    d. O(nlogn)
    e. O(n^2)
    f. O(n)
    g. O(n)

II.
    a.  function getMax(a) {
            let min = a[0];
            let max = a[0];
            for(let i = 0; i < a; a++) {
                if (a[i] > max) max = a[i];
                if (a[i] < min) min = a[i];
            } return max-min;
        }
    
    b. 
        let prev = 0;
        let prevBroken = null;
        function breakSomeEggsAndGetF(n) {
            let floor = n-1;
            while (floor > prev) {
                const egg = new Egg;
                prevFloor = floor;
                egg.dropFromFloor(n);
                if (egg.isBroken === true && prevBroken !== false) {
                    floor = floor/2;
                    prevBroken = true;
                } else {
                    floor = Math.abs(prevFloor-floor)/2;
                }
            }
        }

III. 
    a. 