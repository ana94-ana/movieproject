<script setup>
import watchlist from './components/watchlist.vue';
import Search from './components/Search.vue';



      const movies=[
                    { 
                        id: 1,
                         name: "ყველაზე ჭკვიანი ცხოველები მსოფლიოში ★ ტოპ ფაქტები ★", 
                         url:"https://www.youtube.com/watch?v=Mra2YR_wWXA", 
                         description:"ვიდეოში გაგაცნობთ ყველაზე ჭკვიანი ცხოველებს მსოფლიოში,10. კატები,9. ვირთხები,8. სპილოები " ,
                         cover:" http://kabisashvili.blogspot.com/p/cxovelebi.html "
                    },
                    { 
                        id: 2, 
                        name: "10 ამოუხსნელი ბუნებრივი ფენომენი  ", 
                        url:"https://www.youtube.com/watch?v=x2wIhpy6sfA  ",
                        description: "ვიდეოები იქნება მრავალ თემაზე, დედამიწა,გალაქტიკა,კოსმოსი,მეცნიერება,თეორიები,სამყარო,ცხოველთა სამყარო,ფრინველები,მცენარეები,ქვეწარმავლები,ანომალიური მოვლენები, ",
                        cover:" https://yourshot.nationalgeographic.ge/saqartvelos-veluri-buneba/?contest=photo-detail&photo_id=1358  "
                    },
                    { 
                        id: 3, 
                        name: " სახიფათო ცხოველები უწყინარი გარეგნობით ★ ტოპ ფაქტები ★ ", 
                        url:" https://www.youtube.com/watch?v=VA6WpcxNT-U ",
                        description: "ვიდეოში ვისაუბრებთ სახიფათო და სასიკვდილო ცხოველების შესახებ, რომლებსაც საკმაოდ უწყინარი გარეგნობა აქვთ. ",
                        cover:"  https://yourshot.nationalgeographic.ge/saqartvelos-veluri-buneba/?contest=photo-detail&photo_id=1354"
                    },
                    { 
                        id: 4, 
                        name: "10 ყველაზე ლამაზი ადგილი დედამიწაზე  ", 
                        url:" https://www.youtube.com/watch?v=05P_dKyAcr8&t=6s ",
                        description:" 10.ყინულის გამოქვაბული ვატნაიიოკიუდლ9.ბამბუკის ტყე საგანო8.ზღვის გამოქვაბული ალგარვე7.მთა რორაიმა6.იგუასუს ჩანჩქერები",
                        cover:" https://yourshot.nationalgeographic.ge/saqartvelos-veluri-buneba/?contest=photo-detail&photo_id=1357 "

                    },
                    { 

                        id: 5, 
                        name: " 10 საქართველოს ყველაზე ლამაზი ადგილი ", 
                        url:" https://www.youtube.com/watch?v=6EboEbD60xc ",
                        description: "ვიდეოები იქნება მრავალ თემაზე 10 საქართველოს ყველაზე ლამაზი ადგილი  ",
                        cover:" https://yourshot.nationalgeographic.ge/saqartvelos-veluri-buneba/?contest=photo-detail&photo_id=1359 "
                    }
                  ]
  


</script>

<template>
  
  <div>
   <Search/>
   <watchlist :data="movies"/>
  
  </div>
</template>