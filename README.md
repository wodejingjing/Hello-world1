# Hello-world1
this is my first
public static void main(String[] args) {
    int[] arr={1,5,7,2,3};
    bobbleSort(arr);
    print(arr);
}
/**
 * 1.返回值类型 void
 * 2.参数列表int[] arr
 */
public static void bobbleSort(int[] arr) {
    for (int i=0;i<=arr.length;i++){
        for (int j=0;j<arr.length-1-i;j++){
            if (arr[j]>arr[j+1]){
                swap(arr,j);
            }
        }
    }
}
/**
 * 1.返回值类型 void
 * 2.参数列表int[] arr,int j
 */
public static void swap(int[] arr,int j) {
    int temp=arr[j];
    arr[j]=arr[j+1];
    arr[j+1]=temp;
}
/**
 * 1.返回值类型 void
 * 2.参数列表arr
 */
public static void print(int[] arr) {
    for (int i=0;i<arr.length;i++){
        System.out.println(arr[i]);
    }
}
