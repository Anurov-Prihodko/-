-----portfolio-btn--------

.portfolio-btn-item {
display: flex;
justify-content: flex-start;
margin-bottom: 70px;
flex-wrap: wrap;
}

--------work examples---------

.work-examples-title {
@include font($fs: 18px, $fw: 700, $ls: 0.06em);

line-height: 2;
margin-bottom: 4px;
color: $text-head-color;
}

.work-examples-text {
@include font($fs: 16px);

line-height: 1.875;
color: $text-main-color;
}

.tehnocrack-text {
font-family: $text-font;
margin: 0;

@include font($fs: 18px);

line-height: 1.556;
color: $white-color;
padding: 77px 24px;
}

.tehnocrack {
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
background-color: $card-background;

overflow: hidden;
transition: transform $time $function-time;
transform: translateY(100%);

.work-examples-link:hover &,
.work-examples-link:focus & {
transform: translateY(0);
}
}

.work-examples-link {
transition: box-shadow $time $function-time;

&:hover,
&:focus {
box-shadow: $work-examples-shadow;
}
}

@media screen and (max-width: 767px) {
.work-examples-list {
margin: -30px;
}

.work-examples-item {
margin: 30px;
flex-basis: calc((100% - 30px) / 1);
}
}

.tehnocrack-card {
position: relative;
overflow: hidden;
}

.description-foto {
padding: 20px 25px;
}

.work-examples-img {
object-fit: cover;
width: 100%;
height: 100%;
}

.work-examples-item {
max-width: 450px;
outline: 1px solid $border-work-examples;
}

@media screen and (min-width: 768px) and (max-width: 1199px) {
.work-examples-list {
margin: -15px;
}

.work-examples-item {
max-width: 354px;
width: 100%;

    margin: 15px;
    flex-basis: calc((100% * 6 - 15px) / 2);

}

@media screen and (min-width: 768px) {
.work-examples-list {
display: flex;
flex-wrap: wrap;
}
}

.tehnocrack-text {
padding: 49px 24px;
}
}

@media screen and (min-width: 1200px) {
.work-examples-list {
margin: -15px;
}

.work-examples-item {
max-width: 370px;
width: 100%;
display: flex;
flex-wrap: wrap;

    margin: 15px;
    flex-basis: calc((100% * 6 - 15px) / 3);

}

.work-examples-list {
display: flex;
flex-wrap: wrap;
}

.tehnocrack-text {
padding: 63px 24px;
}
}
