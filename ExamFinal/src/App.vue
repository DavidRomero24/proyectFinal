<script setup>
import { ref } from 'vue';

let like = ref(28)
let noLike = ref(3)

function addValue(){
  like.value++
  console.log(like)
}

function addValue1(){
  noLike.value++
  console.log(noLike)
}

// parcial discord
let index = ref(0);

let mensajes =[{
  name:'Marco Perez',
  mensaje1: 'Hola como estas',
  mensaje2: 'fulbito?',
  mensaje3: 'toca ir a la u?'
},
{
  name:'Juanito Alimaña',
  mensaje1: 'que haces xd',
  mensaje2: 'un lolsito?',
  mensaje3: 'juguemos valorant'
},
{
  name:'Anonymous',
  mensaje1: 'te estan hackeando',
  mensaje2: 'queres saber quien es?',
  mensaje3: 'si por favor'
}
]

function doClickMaestroSplinter(indice){
index.value = indice
}


// parcial turnos 
let indice = ref(0)

let refcodigos = ref("")

let codigos = ref([['XDADAL1', 'SDSADA1', 'SJDAD01'], ['UWASDAS'], ['ASDAD123']]);

function addCodigo(indice){

codigos.value[indice].push(refcodigos.value);

}

function deleteCodigo(indice, index){
  codigos.value[indice].splice(index, 1);
}

</script>

<template>
  <!-- parcial instagram -->
  <div class=" w-[40%] mx-auto shadow-md shadow-gray-700 px-4 py-2 mt-12 mb-12">
    <!-- 1 -->
    <div class="block mb-5 ">
      <div class="flex justify-between">
        <h2 class="text-center font-semibold ">Historias</h2>
        <span class="text-white bg-blue-500 px-1 rounded">Todas</span>
      </div>
      <div class="justify-between flex pt-5 ">
        <div class="block">
          <img src="https://media.vogue.mx/photos/5e28d7901620aa00083efea6/2:3/w_2560%2Cc_limit/camila-cabello-con-peinado-de-ondas-largas.jpg" alt="" class="w-24 h-24 border-blue-400 rounded-2xl border-solid border-4 ">
          <span class="opacity-50 ">Camila</span>
        </div>
        <div class="block">
          <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAoHCBYWFRgWFRUZGRgZHBgcGBkaGBgYGRkYHRoaGRwcGhgcIS4lHB4rIRgYJjgmKzAxNTU1GiQ7QDs0Py40NTEBDAwMEA8QHxISHzQrJCs0PTQ0NjQ0NDQ0NDQ2NDQ0NDQ0NDQ0NDQ2ND00MTQ0NDQ0NDQ0NDQ0NDQ0NDQ0NDQ0NP/AABEIAOEA4QMBIgACEQEDEQH/xAAbAAABBQEBAAAAAAAAAAAAAAAAAQMEBQYCB//EAEEQAAIBAgMEBwYCCQMEAwAAAAECAAMRBBIhBTFBUQYiYXGBkbEyQlKhwfAT0RQVYnKCkqKy4TPC0gcjU/E0Q2T/xAAaAQACAwEBAAAAAAAAAAAAAAAABAECAwUG/8QAKxEAAgIBBAEDAwMFAAAAAAAAAAECEQMEEiExQSIyUQUTYXGBsRU0QqHw/9oADAMBAAIRAxEAPwDyiEISACEIQAIQhAAhCEAAwXnC0HkMlC09TLMJcW85XURrLZUOiLqx5b/PhKylRpCNkOtQPK0n9HqbCoBbf6S92b0eOUFydeA+sv8ADbGVNVWx5xeWZNUMRwtOzzbbGGyVWHC+kYpU7z0DavRkv11BuSb31HzmdfZhRsrrlPAj2T38paOZNUVlgadlfSY2sw09JBxKAntHzl3iaOXhKfFL5ibRafKMZJrhkGdxGEUGXKMIQhAqEIQgAQhCABCEIAJCEJICwhCQAQhCABCEIAEIQgAqDeYD1inRYce6Qy6XBJwSi5Y8PWbTojsz33Fyxv3DhMTmsoHMi/n/AInrPRvD2opp7oimeTocwRRd4agBwkoIOU4TSOBoqmMNDbpKPauzlcHT/wBzQGRcSlxJbBHm2KSxam+8XKnmvKZzHplOo7+0TY9LaIW1RSMyG+/UjiJm9qoD1huIDL+62tvA6eUZwsWzRRRMmpHlEtY/fjO2OgPLTw4fWc1BpGhWjmEQGLLGYQhCABCEIAEIQgAkIQkgLCEJABCEIAEIQgAQhCAHTcIlOcsY5QGolWXj2S8LhXq1FRLXJ3ncLCehYXD4ukos6ta2gYehmO6PKwqhlGoDegkt/wBLq1Fvnyu+WygkgX004XudTF53J1wNwqMb5NxhtvVAQtSmR+1bTz3S+w2IDi4lK+yGwxGWqXRjuYAMp/h0I3crS1wKENlMUnFpjMWmrOcfjxTG654CZnE7TxNQ5QUpg8Sbf5l1tMEl7e6rHt05TK9GtlvXqOcQaiABgSLIAdMtifa97staXxx3FMkkiRiejSOhL1ndje5BAF+wazLYmlZAh1NNmQ/u8PX5TRVcLUoYgKjmqjXubAMtzxy6Hv0kPbWzmF2Pv3v3jUS9uLpsq0pRtIxjrZiDx+/W04Efxaa/e/jI7c+frxji5EmqZysWDDXvhLozfYQhCBAQhCABCEIAJCEJICwhCQAQhCABCEIAEIQEAOWj9I2+/vlGBvjlFGdgq72IA7zKy6NIdm76C4TNmc9g8d59Zuf0BDrlF+f+ZnOiVLImQ7wbHvmwpm4nNlK5M6sY1FEdKIEcoe3ePOLCNYYXMq3ZFEZx1yY7+COQ8ozi+q0m0xpJQUQzhBvtM/0gUBSOE1dQzMbcwz1CVQXsMzc7dg4mEeWX20jzjadKzHt1/P8AOVg3Ectfzmp29swpTRxfUda/BuImWzag+cfxu4nNzRqQNEnZX79JwJqjCSCEISSoQhCABCEIAJCEJICwhCQAQhCABCEIAEIReBgShubPoZ0eq/i56tJ1CgZcykXJ4+kY6AbF/Gr/AIri6USD2M59keHteU9cZVFi7WvuG7yiubJXpQ3gxf5MylPOtWoSjKuYAEggN1Rcg8r+k0GErgidJiEcHK9wCRY67iRv8JAKFGBHsN7PYeUUkvI/F+GW9XVTK6hinVz1OrbQ8fKSjWAW5MhLtSmCdfT0lewSfhEepiajOwZCFt1eZPoBLjDCyAHeALyrfatMm1/HT0k1K4K6SegaflHWIqWEoy9ZXzohdSLEDjY8Dzk/FPpKLafSNsKt1UOL7i2Ui/gYQty4JbSRcbT2amJpNoUcjcRY37R9Z5BjMKyOyMLEEgjtE9t2DtWnjaQqUwRbRrgghrC4vx38Ji+n+x+t+Mo5B+/3T8reIjOKW2VMUzRU42jz0HhBhOqiWN5zGxFqxIQhLFAhCEACEIQASEISQFhCEgAhCEACEIQAIGE1PQHAJUrNUcX/AAlVlXgXJIBPdY+JHKVnLbFyZfHHdJRN70O2d+j4enTYWdru45M2uU9oBA8JYdL8QEw7MVL5bNYC+438JI2et2vJG16iqjFiAApvflac5Pc22dRLakkeA0dsVVdmWoyBmJIViFAY33dl56xszbCiiqVrXtoQCQeRGmhnj2GwzVamVF1YkgDcAT6C89N2Lh2oqqVNbWCtz03GMahJJUZaVyd7uUWWOLOg6xUHeBv8YzgNnlVPXLX33CX+am0s6QDacJ0dj39liPGKRk0OKUaplNtPAAgEvbkBluPEASdsakVQ3LEHdfgJMXY6jViT3wqkKISk2Q5RqkMYpp5l0v2iXfIvsrvPAnkDxtNvjtoKaiUc3WdsunAfYt4yR0i2Cj4dlCgFVuvMMBoZrhajLc0ZZYuUWosk/wDS/CumDGcWDMWTnkYAgnv1PcRLjauFWoHRtzIw9LSdspAtJQosAqgDdYWEj4k9eVnK3uKRjS2niONo5WKngSPEXErmFjNd0ywIRy67ixuO3f8AfdMs63F+IjuOW6NiWSO2VDbCciAaBF901TMZKwhCEkqEIQgAkIQkgLCEJABCEIAEIqgncL90QiBO11YTTdAa1q7rzpm/gy29TMwTLzoPUtigPiVh6H6TPLzBmuHiaPZ9lpoDzjPSmhnw9ZbXLU3A53ym3zkrZ3siO45bqR2RCHR0H2eWdA9gOrs9ZMtwAoNteJOnhLzpnjRSo5R7T9VeY5nw/KXWGWyLzA0nnXSTFNXxoQ7kyrbtPWY+nlNU3N2yVUEkv0NDszaToq/iaggdftt73Lvmrwe00YXDCZ7DUxltGa2xFOqFkP7JIHlF7VmtJmmxu0kUXLCYzau3i7ZKd2PADnHD0dLe3VZh98zLPB7LSmLIuvEnUnxhcVz2FJdGYwuy3VhWqG7ghlHBSNReejZg6Lb3reRlDUoi9ppMBRAygbgP8S25y7I4XRbILLKvHm1zLW+kp9rHSEjJdnlnTjEn8SmOwk9p0/zM2r2PYZYdLq2auf2VA9T+UrFTT07I9iVQQplTlN0d1qPvLu9IyJIwtWxsf/ckvhQ2qS7ddkRxblaIO/fviMpElrT1ysLNwB0v3Hh4xQwAKsuu63Pu+FvkZKkDwfkhQjtajYBhqp3Ht5HkY1LC8ouLpiQhCSVFhCEgDqlTLsqLvYhR3k2E3WC2FTy5Uo5yNGquPabjkU8JD6C7LF2xLjq07hBze2p8L28TNhS2kDvA8JDrydz6dpVt+5JXfVlRh9gIp3KOdgJnuk2FS9kHWAJM3teouUHcTumD27TK1zrcEA39ZSa29HRyY4yxuLXD4MqaTHgQO0Wv3X3+Ev8AongXp4qmzKVHWGuh9luHDxkzZ5FPrqASbXvv/hYarvlxsJkqVxlDhlBYgqLW3e0D2ymSdxZzl9Pjjjuk+fB6Ngl6ojmI3Qw4sojeJrADWJR4RklbKhWsrD4SfI6j1nmiMDj3bhma3eAB9DNltzaoQOQdToo5mZPYiWfOddde73vWbQumbrA5/wAmrw1zuGks6SRyhTWwtHwsWaKWcLTg9COCdwSIZU4mkFux0A1l7gGub90zXSCvYBBx1PcN3z9JZdHcaGQA7xofCabajZu8L+2p/JpidJTbWHVlxTNxIG0aNxaVYquzxDadBnrOQLnM1wN9gbfSWGyNgvWNgMoW2Ytcb92h3yJtjDNSxdUMLdYkdza3HZvnVAOFZVYhbg2BtHk0kjfBCM220O9IOj5pEFGDDsO7vlRhcUUbXQ/I98sFBvqTfvndXBq4Fxa5tm/OTuXXgnJpG3vxcP4LNWo4hcjgDTRh7SHnce0v3rM/tDAVKRIbrKLWYagqdx7RJ1fYGJoWdFLrvDJ1rfwjWS8FtRHGVlGYX6h0F+OW+6/wnjLdGTSyenIql/Jmlqkcbq2jD08ZyRNFtHYAdfxKB0IvlPzHYZmxcXUixHA/MS6ENRhlB1L9mEIQlhSmLOkQsQqi5JAA5kmwnMu+h2Gz4unfcmZz/CNP6isg0xQ3zUflm6NJaFBMOvugZu1jqT4kmcpgWFmJsDuHEmPsM9TQcbluySWpswLKQoX2cwJB56DnKtWz1yrHFRRS7UrZLZyByXebd0zuMqBySt9O4eVyJcbX2dXqnMchA+E3IHdaQ6WzC1y7AAC5Y2ACjixmcrbqi0raIFEkAZxobW0sbEXE3PRLBKqF7aufkNB9ZiqgVtEJIykrcWNgdNL6A6mei9H6WSmingov321iuZ0qE88vQki/U6Ss2q9lJlgDM50uxOSi7DfbTv4TNc8CEV6jD4pjXqm3srcDsA3nxk7DUgoAHD1jGxqiMhOitufs4A/um/hLJqeW/PQ/Q/SORjS4O3ghHami52PWumU7108OH5eEt1EzGArZHB4bj3TVU4rljtkc7V4tk+OnyIBOWMkESu2tWyoeZ0/OUjFt0YY4OUlFeTNY+pncnhw7huj+wa+SqBwbTx4RhEvcxLCmpdvbsSig2NwMxtzbKGIHYOcccfTR2c0YwxNPpI9BpYkAW4x9sOzrmW3ADf7R908jquu7rCZTZFR2vqWN311sylwyOvAaZNNPYM1C1nCkCwub6amwFgPAW8hMEor3HnJuTfpM9j9h0MShzqodgwFQjVSL5deFtT23nl65luGFipKuORBt6z1XaFBwrZHZWItfQ9uoIsZgKlAms4e2ZgrMLqd6ge7pwvaXxyUvShvRqSnTfZGwwRhZ9/Zp85NTAixAzEHu0nGE6OErUdqjJkJygcdSALDdu3ybsbFvRpNnF+sMhYXNrda3Mez5zbbXZ1Mc5PhxNNg8YgRVVhe1iDoRpyMr9p7Pw9c/92nZuFROqwPPTf4yrfbTHlbsUflH8PtbWzKLdgt8txmqyLos9MpJ7lZ3htkvh2zA/jUTvIFqidpUe12keXGVXSvYaOPxqZAYrfTc1vzHpNbTxGUBguYEXBU6eR3Sq2pXFTQKVvv00JlnSXArPTqcXF8o8uyHkYTY/qjs+cWUtnO/ppj5tf8Ap7hL/jVT+yg/ub/bMVPV+iWE/DwdO+97ue9tR8rCaIW+nw3Zt3wWCURoo3sde7jJuNoEoFU21HyjGAN2Zjw0HrExW0LdVdW3CHFHdlucuPAxisqtZbZ2spPLnaZDpBj7uKaLmpo134B2HAke6N3ffsmgrIy9UG9WoSAb+wu9m7wPmRIuKxq4cBPwQF3ai9wO075SXXwaONqrKnYmHLMCUA1uW1BIPDu0noGA0Ezeyav4hLgtkJ6qG1kI0IW3CabDCc3NJOVLwI6iVuvgnBpkOnb/APaA5sPz+k1ZaZHpsb01/fH1kw9yMcauaMjhlKkMpsRu7eYI4g8pd4avmUcOFvhJ90k+6d6nwlWgkiibG/gRzB3g/fKNRdHagq6LULYzS7KqXSx3rp4cPlM5Q1A1vxv8S9v7Q3HzlvsurZwPi0+o+vnDLHdGymrhvx35XJeMZndt1LsBy9T9iaCsZm8YMzHvMwwRuV/AloY3k3PwRqZyqWJAAH3990osVWZ3znS3sDflHb2neZZ49r2TgLE/QfXxHKQXoxiT8HTmt3ZruiGJz0iSAGzvmsLC5Nxp3ETRkzD9EauV3TnZh6H6Tao1xE5qmziZ4bZtIj4lLzLbVwgD5wNRv7prKkrcbRuJmpOMlJFccnGSaM6drrRLkrmzBMi8LAHUnvLfZlM9apiH592iqOQ5CS9obHZ3PXIUKMi27dRfx7/KPUtnMq9dxTQcNwPhxPfOkpPIr8HWwyT9QUcBTX23ufhGvzlhhaVI+zTFhvZtZUDHUl9hGc82Nl8oxia1eqLM2VfhXQeclSivBvJtrizQ1tuU06qgEDcN0YG1nbrLRXKeNifnM4uzLbmkrDrUQ6NDc/JkoLyv9lp+sKnwL/J/mLIf6ZV+IwlrI2r4MDRp52VR7zKv8xA+s9tdFSmF3BQAO4C08d2Gt8TRH7aH+U5vpPSdo1FqKCzhV1046HTT73y90cb6Vj3Jy/IlXaqUwRmuSb2XX57vK8rH2pUa/wCGhUcbC5Pex1nDNSU9VWY9psPlGcTiqjDKFyryUWEylL8nf+3FDeE22ablmXNoVIN7gG17HhuEmv0kVwEOHzg6ZWJO/l1dJAweymc2LBe/fLajshabLrmO+8pulGDfgXy+lNstdnUgoAVQo4Abh2S5oSBhksJPoznLl2cqbHnbSY/pe1wg/b+hmsqtpMf0oN2QdrH5f5m0Pci+nVzRU0qcdNOPUBJLUxaOUdpIj4SqQct7XN1PJtw8DuPeOUtKD2Icdh7rHUHtuCJU16NxcSThMTmU8yDf94WVvO6HxMPwwfKo12IfQSivvJ3fZPyBlkHugPYJS4kmwA7j/EQD/SrTDTPsR0fG4YWkWJY72JPnwj4wvZJWBpXF5IYRpR8jrnzRWYOnkqq3PTz+xNhh30mYxam1xvEvsFUuAeYEV1ENskzn62PKkTXkSqslGMPFmhBFHjqJ3qbEbj2yiw+y2cl69XMwJ0JsB4HdNZiadxKHH4JWIzLexvaXw5djp9DWHLtfPRFZaXxobfDdv7QY0z0v/IPJ/wDjLajXGUqKYU6AC4NyeXZGqmyL6zoVauPJ045LV2VRroPfXziHGUwNXXzEcxeAymV1WgvGUdoJJtcHX62o/F/S35Qld+jryhJ3C+3J8kDo+t8QnZmP9J/Ob/DYRWIzGwnnmyKuWshO69j/ABAr6kTZPUIEtJ0+RH6S19qSXdl1VWglxvIkGlZ23WEqc7E6yRTqvuUWlHK30diMa8lzWwlMrqd3EaGJs+lbiT3m5kDD02J6x8JdYVIpqMu70o52py7ntT4ROpCS6cjIJKQaTGKEmziudJktui9RO5v9s1Vc6TOYqnmq9y+p/wATfErkhjSK8iI9KlpH6VjoRJlKgBHWwY9ob4+os6zmkQaCAOVI3jSQMRS/CrlfdcXXsYA38wT5CWWNGVkf4TY9xibcpB0BXR1sy9tt4Hba8hrgq27VE/B6017VHpKXGPlfxPyB/wCctNi4gPTHZpbl9/lIFdA1fKeDX/h6pP8AY0Uwxam0J6dOGSSZdYRAqAHeBcxik2Yk8LxK9fKhY8d3dwjmz06oMe80MdJyY1iEvcSZsl7oBxXT8oj07mcYYZWPI+sx1ELjfwY56lj/AELhDG6gi02nTic+jmEVxK/EUZZNGaqSkkSmVISxDDeJ1VxTH2Ru37pJdJHxOHuPvXvmuDO4On0M4cu189FVUqs50F+6Ra2Dt7bBe9gJJBfc7Iq3sRbILd+cSI+zabE/h2YX91gx8QI/2r7OnutXEhZKX/kX+YRYn6pHL+mEP2MvUY+bahiM6I494AnsPH53mJkzZ71GIpq5CsbkcAOJ7JeatHndBqXhm1V3xx8mvWSMMGv1Tbtkamiqtycqra537zbxYmXNFBvUWGlhxt29sUyy2xs9Bmy7YV5YtKnLTDppI1FJOQRJcs5kmO011kk7ozTEdczRFGRsQdJV0EuzntA+v1lliDpIWAI64/aPosZ0y9Y1peHY+tOJWUlbDeN0XEMbaSvbHsu+x79/nHm0ux9RlLlHQfOpRhrI1FsylGNmXUHlbd4RuriCWzAZTO2e5V1AJ3Mvf9DM7N9tf95Fwd0JIFuXw89404EX7eyc4Uddy3tNcDUGwJ+EbjacuLg3GUa6EWPyFjHVvl6t7sBrrYDd4GRSuwcFe7yK6BqgDAsBuVdwA+I8ZaUiSdNAOEZ2fSCDfcneez6CO1MWi318polXLMJNt0kTBGaxHlK/9dJew9RG6uPDHQW8YSlGSoqsMn2i9w9TSSQZU7Or5llirTlPh0cucdsmmDrGzHXMYJkMqNVEjRWSzrGHW0o4hZUY/Coesy7gdbXIHZKX8FWVWWzK17MBbcbd4NxNRiBpMngfxUDBMrpme9P3wMx1A590a087Tix7Szk7j4Osh+Jv5jCH6R/+er8/+MI1wN0YSXnRmldnbjoo8dT9JRzQ9EnsXsLlQXUc2Ctb5iaS6PM/T0nqFf5LDaNTNUWgtsqsCx+JhqfLUCarDjQTLbIpqWd332YrcHU6kt4dvOabAPmAnP1KbSZ29VB8SLGmkeWcoIAzBcIRfZJQwZpwpiMZYgaxDaSk2fiCarKOBPoJZY+uFUnlKHow+aozk2GVmJPC50jOn9w5pVVv8GiquAdfGNPh0biJHrbQpMSoex5yG9K+6qPnHXJfqdCEX80TsTgFK6b+UpWLUW10U893jJX4T8ai255vpOqhVVINTMe1rAeBIv5ykqf4NV6eG7OVJBu1lJ94G6nv+zF/HtbrHtIXNfusvpINKkoIYZNQQMoYg/ykrfuMeUmw1I04MoPzN5VMm0d43bBsVQdY7yRY27uEgpSZ/bYns3CSaVl9lA7H2s+Zah7bMet4R5craKCjD3W490GnLyEaS4Qn6OqLuA8pzfiJBx+IObLxG/snNKtaVtXRbsvdlVyrWO4+s0StMXSxGtxvGtpqMFiA6gjjFc0adnK1mPbLd8k+84aCtBpiI0IDOKkWc1DpIAg4t7Ayiw2FVg/VJYNddLZudm3gjs7JM2riOA4WJ9QO7SRKFSodFBBvmYi1gd+h+98b00aW5+To6WDjFy+RjM3x1/MQk39YVea+UI1SGbZ5lNL0I/1W7h6PCEtLo8x9P/uIk7D7qn7v+5ZoNn+03eP7ViwiWf2HotZ7EXK7oCEIqcpjqzl4sJKAoOkf+i/7plPsf2Kv7qf3QhGsA/pPJXLvPeZLpQhNUdIKu6Vn/wBo74QkyMshcN/q+foI5j/9I93+2EJPgv4E2Z/8bxHrLh/apffCEJaBEfaUdb2637xkVYQmT7NYkjD+0Jpdh+x4t6xITPN7RPXewuUnRhCKnJOWjVbdEhIAzGL9o/v/AEWM4f2TCEfx+1HYw+xEeEITQk//2Q==" alt="" class="w-24 h-24 border-blue-400 rounded-2xl border-solid border-4">
          <span class="opacity-50 ">Maria Fernanda</span>
        </div>
        <div class="block">
          <img src="https://www.shutterstock.com/image-vector/scary-paper-bag-head-halloween-600nw-1789448435.jpg" alt="" class="w-24 h-24 border-slate-400 rounded-2xl border-solid border-4 ">
          <span class="opacity-50 ">Señor Equis</span>
        </div>
        <div class="block">
          <img src="https://www.biografiasyvidas.com/biografia/j/fotos/juan_carlos_i.jpg" alt="" class="w-24 h-24 border-slate-400 rounded-2xl border-solid border-4 ">
          <span class="opacity-50 ">Juan Carlos</span>
        </div>
      </div>
    </div>
    <!-- 2 -->
    <div>
      <div class="">
      <div class="flex justify-between py-2">
        <div class="flex"> 
          <img src="data:image/jpeg;base64,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" alt="" class="rounded-full w-14 h-14 ">
          <div class="block px-1 ">
            <h2 class=""><strong>Mariano Pérez</strong></h2>
            <p class="opacity-75 text-sm ">Hace 10 minutos</p>
          </div>
        </div>
        <span class="flex text-red-700 place-items-end"><strong>Reportar</strong></span>
      </div>
      </div>
      <div class="">
      <img src="https://cdn.redcanina.es/wp-content/uploads/2019/02/12102930/golden-cachorro-e1549967733842-1024x650.jpg" alt="" class="w-full rounded-2xl ">
      <div class="flex mt-1">
        <div class="flex px-3">
          <svg @click="addValue" class="w-7 " viewBox="0 0 256 256" xmlns="http://www.w3.org/2000/svg"><path fill="none" d="M0 0h256v256H0z"></path><path d="M128 216S28 160 28 92a52 52 0 0 1 100-20h0a52 52 0 0 1 100 20c0 68-100 124-100 124Z" fill="none" stroke="#ff0000" stroke-linecap="round" stroke-linejoin="round" stroke-width="16" class="stroke-000000"></path></svg>
          <p class="" >{{ like }}</p>
        </div>
        <div class="flex">
          <svg @click="addValue1" class="w-7" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg"><g data-name="1"><path d="M242.28 427.39a43.85 43.85 0 0 1-13.1-2c-18.22-5.69-29.87-21.64-29.69-40.62.16-17.35-3.15-32.5-9.83-45-8.19-15.33-21.83-27.13-40.55-35.08A15 15 0 1 1 160.83 277c45.4 19.26 69.14 56.6 68.65 108a12.28 12.28 0 0 0 22.33 7c28.34-41.71 3.47-87.63 3.22-88.09a15 15 0 0 1 13.12-22.27h141.64a14.22 14.22 0 0 0 0-28.43h-20.45a15 15 0 1 1 0-30A14.2 14.2 0 0 0 403.55 209a14.23 14.23 0 0 0-14.21-14.21H368.9a15 15 0 0 1 0-30 14.21 14.21 0 1 0 0-28.42h-20.45a15 15 0 0 1 0-30 14.21 14.21 0 1 0 0-28.42H261.8a111.69 111.69 0 0 0-39.07 7l-67.5 25.07A15 15 0 0 1 144.78 82l67.5-25.07A141.5 141.5 0 0 1 261.8 48h86.65a44.25 44.25 0 0 1 40 63 44.27 44.27 0 0 1 20.45 58.43 44.27 44.27 0 0 1 20.44 58.42 44.21 44.21 0 0 1-19.59 83.84H290.11c6.77 23.11 11.23 60.85-13.48 97.22a41.21 41.21 0 0 1-34.35 18.48Z" fill="#ff6a00" class="fill-000000"></path><path d="M155 305.85H69.13a15 15 0 0 1-15-15V85.21a15 15 0 0 1 15-15H155a15 15 0 0 1 15 15v205.64a15 15 0 0 1-15 15Zm-70.84-30H140V100.21H84.13Z" fill="#ff6a00" class="fill-000000"></path></g></svg>
          <p class="" >{{ noLike }}</p>
        </div>
      </div>
      </div>
    </div>
    <!-- 3 -->
    <div class="flex justify-evenly bg-slate-200 rounded-2xl p-3  ">
      <svg class="w-12 hover:bg-white rounded-xl" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><g data-name="user people person users man"><path d="M23.74 16.18a1 1 0 1 0-1.41 1.42A9 9 0 0 1 25 24c0 1.22-3.51 3-9 3s-9-1.78-9-3a9 9 0 0 1 2.63-6.37 1 1 0 0 0 0-1.41 1 1 0 0 0-1.41 0A10.92 10.92 0 0 0 5 24c0 3.25 5.67 5 11 5s11-1.75 11-5a10.94 10.94 0 0 0-3.26-7.82Z" fill="#1b7cde" class="fill-000000"></path><path d="M16 17a7 7 0 1 0-7-7 7 7 0 0 0 7 7Zm0-12a5 5 0 1 1-5 5 5 5 0 0 1 5-5Z" fill="#1b7cde" class="fill-000000"></path></g></svg>
      <svg class="w-12 hover:bg-white rounded-xl" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg"><g data-name="1"><path d="M395.49 450H125.8a15 15 0 0 1-15-15V197a15 15 0 0 1 30 0v223h239.69V197a15 15 0 1 1 30 0v238a15 15 0 0 1-15 15Z" fill="#1b7cde" class="fill-000000"></path><path d="M445.11 261.65a15 15 0 0 1-10.61-4.39L260.64 83.4 86.78 257.26a15 15 0 0 1-21.21-21.21L250 51.58a15 15 0 0 1 21.21 0l184.51 184.47a15 15 0 0 1-10.61 25.6ZM304.15 450h-87a15 15 0 0 1-15-15V305.48a15 15 0 0 1 15-15h87a15 15 0 0 1 15 15V435a15 15 0 0 1-15 15Zm-72-30h57v-99.52h-57Z" fill="#1b7cde" class="fill-000000"></path></g></svg>
      <svg class="w-12 hover:bg-white rounded-xl" viewBox="0 0 512 512" xml:space="preserve" xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 512 512"><path d="M344.5 298c15-23.6 23.8-51.6 23.8-81.7 0-84.1-68.1-152.3-152.1-152.3C132.1 64 64 132.2 64 216.3c0 84.1 68.1 152.3 152.1 152.3 30.5 0 58.9-9 82.7-24.4l6.9-4.8L414.3 448l33.7-34.3-108.5-108.6 5-7.1zm-43.1-166.8c22.7 22.7 35.2 52.9 35.2 85s-12.5 62.3-35.2 85c-22.7 22.7-52.9 35.2-85 35.2s-62.3-12.5-85-35.2c-22.7-22.7-35.2-52.9-35.2-85s12.5-62.3 35.2-85c22.7-22.7 52.9-35.2 85-35.2s62.3 12.5 85 35.2z" fill="#1b7cde" class="fill-000000"></path></svg>
    </div>
  </div>


  <!-- parcial discord -->
  <div class="flex container max-w-5xl bg-gray-700 mt-12 mb-12 justify-between mx-auto rounded-md">
    <!-- perfil -->
    <div class=" bg-slate-800 p-2">
      <div class="bg-[url('https://steamuserimages-a.akamaihd.net/ugc/2059873190232684844/BE10D8DBA2FCE3530A7C20507FCE034F1AD7605B/?imw=512&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false')] bg-cover w-10 mx-auto h-10 rounded-md mt-5">
      </div>
      <div class="text-center text-gray-300">Perfil</div>
    </div>
    <!-- chats  -->
    <div class="p-2 mt-6 justify-between ">
      <div class="" ><h1 class="text-gray-300 text-xl mb-4 ">TENDENCIAS</h1></div>
        <div>
          <div class=" mt-2 rounded-lg"><p  class="text-gray-300 ">#Messi</p></div>
          <div class=" mt-2 rounded-lg"><p class="text-gray-300">#Messi</p></div>
          <div class=" mt-2 rounded-lg"><p class="text-gray-300">#Messi</p></div>
          <div class=" mt-2 rounded-lg"><p class="text-gray-300">#Messi</p></div>

          <div class="mt-12"> <h1 class="text-gray-300 text-xl"> Mensajes directos </h1></div>

          <div @click="doClickMaestroSplinter(0)" class="flex bg-gray-600 rounded-md my-3 p-2 place-items-center">
            <div class="bg-[url('https://pbs.twimg.com/profile_images/1722501239450021888/oYy45eaU_400x400.jpg')] bg-cover w-12 h-12 rounded-full mt-3"></div>
            <div class=" px-2"> <h2 class="text-white ">Marco Perez</h2> <p class="text-gray-400 text-[11px] opacity-70">Hace 10 minutos</p></div>
          </div>

          <div @click="doClickMaestroSplinter(1)" class=" bg-gray-600 rounded-md my-3 p-2 flex place-items-center">
            <div class=" bg-[url('https://pbs.twimg.com/profile_images/1551642306616463364/3spZpRia_200x200.jpg')] bg-cover w-12 h-12 rounded-full mt-3"></div>
            <div class="px-2"><p class="text-white ">Juanito Alimaña</p> <p class="text-gray-400 text-[11px] opacity-70">Ayer</p></div>
          </div>

          <div @click="doClickMaestroSplinter(2)" class=" bg-gray-600 rounded-md my-3 p-2 flex place-items-center">
            <div class="bg-[url('https://i.pinimg.com/280x280_RS/42/03/a5/4203a57a78f6f1b1cc8ce5750f614656.jpg')] bg-cover w-12 h-12 rounded-full mt-3"></div>
            <div class="px-2"><h2 class="text-white">Anonymous</h2><p class="text-gray-400 text-[11px] opacity-70">Hace una hora</p></div>
          </div>
        </div>
        
    </div>
      

      
    <div class="p-2 mt-6 ">

      <div class="text-gray-300 text-xl">{{ mensajes[index].name }}</div>
      <div class="bg-gray-900 rounded-lg w-72 h-20 p-4 mt-6 border border-slate-400">
        <div><h1 class="text-gray-300 ">{{ mensajes[index].mensaje1 }}</h1></div>
        <div><p class="text-slate-700 flex justify-end">25/06/2009 10:50 AM</p></div>
      </div>

      <div class="bg-gray-900 border border-slate-400 my-3 rounded-lg w-72 h-20">
        <div> <h1 class="text-gray-300 mt-3 ml-3"> {{mensajes[index].mensaje2 }}</h1></div>
        <div class="flex justify-end mt-2 mr-3 text-slate-700"> 25/06/2009 10:50 AM </div>
      </div>

      <div class="bg-gray-900 border border-slate-400 my-3 rounded-lg w-72 h-24">
        <div> <h1 class="text-gray-300 mt-3 ml-3"> {{ mensajes[index].mensaje3 }} </h1></div>
        <div class=" flex justify-end mt-2 mr-3 text-slate-700 "> 25/06/2009 10:50 AM </div>
      </div>
    </div>
    

    <!-- PUBLICIDAD -->
    <div class="bg-gray-800 rounded-sm px-5 py-2">
      <div class="text-gray-300  text-xl font-medium mt-6">PUBLICIDAD</div>
      <div class="bg-[url('https://i.ytimg.com/vi/aw1QFNSn5uM/maxresdefault.jpg')] bg-cover h-48 w-48 rounded-md mx-auto mt-4 "></div>
      <div class="bg-[url('https://assets.change.org/photos/3/ub/eh/DKuBeHdNCEOQcyR-1600x900-noPad.jpg?1565970697')] bg-cover h-48 w-48 rounded-md mt-4 mx-auto"></div>
    </div>
  </div>

  <!-- parcial turno -->
  <div class="shadow-md max-w-4xl mx-auto shadow-gray-700 p-10 mb-12 ">
    <div class="text-2xl font-bold text-center ">SISTEMA DE TURNOS</div>

    <div class="flex justify-between mx-auto w-full">

      <!-- IZQUIERDA -->
      <div class="p-5 ">
        <div class="bg-blue-500 text-white text-xl font-bold p-2 rounded-md rounded-b-none ">
          MODULO 1
        </div>
        <div class="bg-gray-300 p-2 rounded-md rounded-t-none">
          <div v-for="(obj, index) in codigos[0]" :key="index">{{ obj }}</div>
        </div>
      </div>

      <!-- MEDIO -->
      <div class="p-5">
        <div class="bg-orange-500 text-white text-xl font-bold p-2 rounded-md rounded-b-none">
          MODULO 2
        </div>
        <div class="bg-gray-300 p-2 rounded-md rounded-t-none">
          <div v-for="(obj, index) in codigos[1]" :key="index">{{ obj }}</div>
        </div>
      </div>


      <!-- DERECHA -->

      <div class="p-5">
        <div class="bg-green-800 text-xl text-white font-bold p-2 rounded-md rounded-b-none">
          MODULO 3
        </div>
        <div class="bg-gray-300 p-2 rounded-md rounded-t-none">
          <div v-for="(obj, index) in codigos[2]" :key="index">{{ obj }}</div>
        </div>
      </div>

    </div>

    <div class="flex justify-between max-w-4xl mx-auto gap-4 bg-gray-300 p-4 py-6 place-items-center rounded">

      <div><strong class="text-xl" >{{ codigos[0].length + codigos[1].length + codigos[2].length }}</strong> TURNOS</div>
      <div class="flex  ">
      <div ><input class="rounded mx-2 p-2 w-44" v-model="refcodigos" type="text" placeholder="INGRESE CODIGO"></div>
      <div> <input class="rounded mx-2 p-2 w-44" v-model="indice" type="number" placeholder="MODULO"></div>
      <div @click="addCodigo(indice)" class="mx-2 bg-purple-600 text-white w-36 rounded-md p-2 text-center ">Agregar turno</div>
      <div @click="deleteCodigo(indice, index)" class="bg-red-500 text-white p-2 w-36 rounded-md text-center">Borrar codigo</div>
      </div>
    </div>
  </div>  
</template>
