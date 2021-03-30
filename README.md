# algorithm
##### 二分算法
##### Markdown
迭代式二分算法
原理：将每一次的结果作为下一次迭代的初始值，这种方法是符合人的正常思维
传入参数：ElemType *array[]      被查找的数组
         ElemType date          待查找的数据
         
给定一个有序数组    arr[]={1,1,2,3,5,8,13,22}
计算数组长度的公式：len=sizeof(arr)/sizeof(arr[0])
数组的总字节/每个元素的字节大小=元素个数

int BinarySearch(ElemType *array[],ElemType date）
{
    int head = 0;
    int end;
    int mid;
    while (head <= end)
    {
        mid = (end-head)/2+head;
        if(dat < bsarry[mid])
        {
            end = mid-1;
        }
        else if(dat > bsarry[mid])
        {
            head = mid+1;
        }
        else
        {
            return mid;
        }
        
    }
    printf("查找失败，数据不存在\n");
    return -1;
}
