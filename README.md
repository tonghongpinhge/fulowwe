# fulowwe
Chọn phần tử nhỏ nhất trong n phần tử ban đầu, đưa phần tử này về vị trí đúng là đầu dãy hiện hành Xem dãy hiện hành chỉ còn n-1 phần tử của dãy ban đầu, bắt đầu từ vị trí thứ 2; lặp lại quá trình trên cho dãy hiện hành... đến khi dãy hiện hành chỉ còn 1 phần tử
void SelectionSort(int a[], int n)
{
	int min; // chỉ số phần tử nhỏ nhất trong dãy hiện hành
	for (int  i = 0; i < n - 1; i++){
		min = i; 
		for(int j = i + 1; j < n; j++)
	   	   if (a[j] < a[min])
		       min = j; // ghi nhận vị trí phần tử nhỏ nhất
		if (min != i)
	   	   Swap(a[min], a[i]);
	}
}
