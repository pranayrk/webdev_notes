<section>
<h5>Selection Sort</h5>
Video by theteachr, ~3 mins
<iframe width="560" height="315" src="https://www.youtube.com/embed/RQy_wFAmSdo?si=P_1LllEhID6CjsBA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</section>
<section>
<h5>Selection Sort</h5>
<pre><code class="language-c">
void selectionSort(int arr[], int n) {
    int i, j, min_idx;

    // One by one move boundary of unsorted subarray
    for (i = 0; i < n-1; i++) {
        // Find the minimum element in unsorted array
        min_idx = i;
        for (j = i+1; j < n; j++) {
            if (arr[j] < arr[min_idx]) {
                min_idx = j;
            }
        }

        // Swap the found minimum element with the first element
        if(min_idx != i) {
            swap(&arr[min_idx], &arr[i]);
        }
    }
}
</code></pre>
</section>
