# Bash Scriping

## Array examples
### Indexed arrays
declare -a array=("ele1" "ele2")

declare -a array=("ele1"
                  "ele2"
                  "ele3"
                  )

array[0]="ele1"
array[1]="ele2"

### Associative arrays

### Iterating arrays
*Iterate through each ele*</br>
for ele in "${array[@]}"; do
  echo "$ele"
done

*Iterate array with idex*
for i in "${!array[@]}"; do
  echo "$i" "${array[$i]}"
done


declare -a array           Declare an Indexed array
declare -A array           Declare an Associative array
declare -a array=()        Declare an indexed array with empty array
array=()                   create an empty array with declaring is valid
array=(1 6 3)              Initialize array with numbers
array=("one" "two" "three")      Initialize array with string
array=("one" "two" 1)            Initialize array with mixed data
${array[0]}                Get first element
${array[1]}                Get Second element
${array[-1]}               Get Last element
${array[@]}                Get All elements
${array[*]}                Get All elements
${!array[!]}               Get All indexes
${#array[!]}               Array length
array[0]=12                Add element to array at first position.i.e index=0
array[-1]=22               Add element to array at last position.
array+=(11)                Append value to an array
${array[@]:k:i}            Get index=1 element starting from index=k

