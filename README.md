# latihan_frontendAmanda
this is my first repository in github
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>latihan 1</title>
    <title>latihan 1</title>
    <link rel="stylesheet" href="DataTables/datatables.min.css">
</head>
<body>
    <table id ="contoh" class="table">
        <thead>
            <tr>
                <th width="5%">no</th>
                <th width="78%" >Nama</th>
                <th width="25%">kelas</th>
                <th width="25%">Alamat</th>
                <th width="25%">No HP</th>
            </tr>
        </tbody>
    </table>
    <script src="DataTables/jQuery-3.6.0/jQuery-3.6.0.min.js"></script>
    <script src="DataTables/datatables.min.js"></script>
    <script>
        $(function(){
            var data = [
                         ["1","amanda aurian rahmadina","XII RPL1", "alamat","085863377702"],
                         ["2","amanda aurian rahmadina","XII RPL1", "alamat","085863377702"],
                        ]; 

            var data = [];

            for (let i = 0; i < 5; i++) {
                data.push([i]);
                for (let j =0; j < 5; j++) {
                    data[i].push(j);
                }
            }
           $("#contoh").DataTable({          
               responsive : true,
               data:data
            });
        });
    </script>
</body>
</html>
