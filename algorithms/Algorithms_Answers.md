Add your answers to the Algorithms exercises here.

I.
    a. O(n)
    b. O(logn)
    c. O(sqrt(n))
    d. O(nlogn)
    e. O(n^3)
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
        let highestGood = 0;
        let egg = {};

        function breakSomeEggsAndGetF(n) {
            let floor = n;
            while (floor !== highestGood) {
                egg = new Egg;
                egg.dropFromFloor(floor);
                if (egg.isBroken) {
                    floor = highestGood + Math.floor(Math.abs(floor - highestGood)/2);
                } else {
                    highestGood = floor;
                    floor = floor + (Math.floor(Math.abs(n - highestGood)/2));
                }
            }
        }

        class Egg {
            constructor() {
                this.maxFloor = 10;
                this.isBroken = false;
            }
            dropFromFloor(n) {
                if (n > this.maxFloor) {
                this.isBroken = true;
                }
            }
        }

        breakSomeEggsAndGetF(20)

III. 
    a. 