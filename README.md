# matrix
matrix

function print_matrix($m){
    for($i=0;$i<count($m) ;$i++){
        for($j=0;$j<count($m[$i]) ;$j++){
            echo $m[$i][$j]." ";
        }
        echo '<br>' ;

    }
}
$t=[
    [1,5,8],
    [2,8,4],
    [9,7,6]
];
function trenspose($a){
    $r=[];
    for($i=0;$i<count( $a);$i++)
        for($j=0;$j<count($a[$i]);$j++){
            $r[$i][$j]=$a[$j][$i];
        }
        return $r;


}
print_matrix($t);
echo"<br>";
print_matrix(trenspose($t));
