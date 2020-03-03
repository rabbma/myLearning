#function

a_function() {
  xxx
  yyy
}

#if condition
if [ condition expression ]
then
  statement1
  statement2
elif
  statement3
  statement4
fi

#while condition
while [ condition expression ]
do
  statement1
done

#until condition
until [ condition expression ]
do
  statement1
done

#exp1
i=7
until [ $i -le 0 ]
do
  echo $i
  i=$((i-1))
done

#for loop
#exp1
for var in 1 2 3 a b c
do
  statement1
done

#exp2
for var in {1..20}
#exp3
for var in {1..20..2}
#exp4
for (( i=0; i<=5; i++ ))

#case
case expression in
  pattern1)
    statement
    ;;
  pattern2)
    statement
    ;;
  "quit")
    break
    ;;
  *)
    statement
    ;;
esac

#file read
while read LINE
do
  echo $LINE
done < filename

#cut awk sed

cut -d[delimiter] -f[field_number] [filename]

awk -F[delimiter] '{print $2}'

sed 's/astr/bstr/' file_name
#replace all matched content
sed 's/astr/bstr/g' file_name
#replace the same file with -i
sed -i 's/astr/bstr/' file_name

