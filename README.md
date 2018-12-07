# DerivadaC
Calculo de algumas derivadas em linguagem C

#include <stdio.h>
#include <math.h>
#include <stdlib.h>
#include <string.h>
#include <ctype.h>

double A = 0, B = 0, C = 0, D = 0, E = 0, F = 0, G = 0, H = 0, I = 0, J = 0, K =0, Calculo = 0, Calculo1 = 0;
double Calculo2 = 0, Calculo3 = 0, Calculo4 = 0, Calculo5 = 0, Calculo6 = 0, Calculo7 = 0, Calculo8 = 0, Z = 0, N = 0, Conta1 = 0, Conta2 = 0;
double Conta3 = 0, Conta4 = 0, Conta5 = 0, Conta6 = 0, Conta7 = 0, U1 = 0, U2 = 0, U3 = 0, U4 = 0;
int number =0, Func = 0, EscolhaDerivada =0;


char F0[7] = "sin(x)";
char F1[7] = "cos(x)";
char F2[7] = "tg(x)";

char U[10];
char V[10];




/*
double A = 0, B = 0, C = 0, D = 0, E = 0, F = 0, G = 0, H = 0, I = 0, J = 0, K =0, Calculo = 0, Calculo1 = 0;
double Calculo2 = 0, Calculo3 = 0, Calculo4, Calculo5, Calculo6, Calculo7, Calculo8, Z, N,

*/
void Menu(){

    /*printf("1:  Ax+B\n");
    printf("2:  Ax^2+Bx+C\n");
    printf("3:  Ax^3+Bx^2+Cx+D\n");
    printf("4:  Ax^4+Bx^3+Cx^2+Dx+E\n");
    printf("5:  Ax^5+Bx^4+Cx^3+Dx^2+Ex+F\n");
    printf("6:  Ax^6+Bx^5+Cx^4+Dx^3+Ex^2+Fx+G\n");
    printf("7:  Ax^7+Bx^6+Cx^5+Dx^4+Ex^3+Fx^2+Gx+H\n");
    printf("8:  Ax^8+Bx^7+Cx^6+Dx^5+Ex^4+Fx^3+Gx^2+Hx+I\n");
    printf("9:  Ax^9+Bx^8+Cx^7+Dx^6+Ex^5+Fx^4+Gx^3+Hx^2+Ix+J\n");
    printf("10: Ax^10+Bx^9+Cx^8+Dx^7+Ex^6+Fx^5+Gx^4+Hx^3+Ix^2+Jx+K\n");*/


    printf("________________________________________________________________________________\n");

    printf("1:  Polinomial de grau 1                    12: y = U^n\n");
    printf("2:  Polinomial de grau 2                    13: y = U.V\n");
    printf("3:  Polinomial de grau 3                    14: y = u/v\n");
    printf("4:  Polinomial de grau 4                    15: y = e^u\n");
    printf("5:  Polinomial de grau 5                    16: y = sen u\n");
    printf("6:  Polinomial de grau 6                    17: y = cos u\n");
    printf("7:  Polinomial de grau 7                    18: y = tg u\n");
    printf("8:  Polinomial de grau 8                    19: y = sec u\n");
    printf("9:  Polinomial de grau 9                    20: y = cossec u \n");
    printf("10: Polinomial de grau 10                   21: y = cotg u\n");
    printf("11: ln U                                    22: y = u^v\n");

    printf("________________________________________________________________________________\n");

}

void Poli1(){



        printf("Voce escolheu Derivada de Polinomio do tipo Ax+B\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);


        printf("y = %.1lfx+%.1lf\n",A,B);
        printf("Resposta:\n");
        printf("y' = %.1lf\n",A);
}

void Poli2(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^2+Bx+C\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);


        printf("y = %.1lfx^2+%.1lfx+%.1lf\n",A, B, C);
        printf("Resposta:\n");
        printf("y' = 2.%.1lfx+%.1lf\n",A, B);
        Calculo = 2*A;
        printf("y' = %.1lfx + %.1lf\n",Calculo, B);
}

void Poli3(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^3+Bx^2+Cx+D\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);

        printf("y = %.1lfx^3+%.1lfx^2+%.1lfx+%.1lf\n",A, B, C, D);
        printf("Resposta:\n");
        printf("y' = 3.%.1lfx^2+2.%.1lfx+%.1lf\n",A, B, C);
        Calculo = 3 * A;
        Calculo1 = 2 * B;
        printf("y' = %.1lfx^2 + %.1lfx + %.1lf\n",Calculo, Calculo1, C);
}

void Poli4(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^4+Bx^3+Cx^2+Dx+E\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);
        printf("Digite o Valor de E\n");
        scanf("%lf",&E);
        setbuf(stdin,NULL);

        printf("y = %.1lfx^4+%.1lfx^3+%.1lf^2+%.1lfx+%.1lf\n",A, B, C, D, E);
        printf("Resposta:\n");
        printf("y' = 4.%.1lf^3+3.%.1lf^2+2.%.1lfx+%.1lf\n",A, B,C ,D);

        Calculo = 4 * A;
        Calculo1 = 3 * B;
        Calculo2 = 2 * C;

        printf("y' = %.1lf^3 + %.1lfx^2 + %.1lfx + %.1lf\n",Calculo, Calculo1, Calculo2, D);

}

void Poli5(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^5+Bx^4+Cx^3+Dx^2+Ex+F\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);
        printf("Digite o Valor de E\n");
        scanf("%lf",&E);
        setbuf(stdin,NULL);
        printf("Digite o Valor de F\n");
        scanf("%lf",&F);
        setbuf(stdin,NULL);

        printf("y = %.1lfx^5+%.1lfx^4+%.1lf^3+%.1lfx^2+%.1lfx+%.1lf\n",A, B, C, D, E,F);
        printf("Resposta:\n");
        printf("y' = 5.%.1lfx^4 + 4.%.1lfx^3 + 3.%.1lfx^2 + 2.%.1lfx + %.1lf\n",A, B, C, D, E);

        Calculo = 5 * A;
        Calculo1 = 4 * B;
        Calculo2 = 3 * C;
        Calculo3 = 2 * D;

        printf("y' = %.1lfx^4 + %.1lfx^3 + %.1lfx^2 + %.1lfx + %.1lf\n",Calculo, Calculo1, Calculo2, Calculo3, E);

}

void Poli6(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^6+Bx^5+Cx^4+Dx^3+Ex^2+Fx+G\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);
        printf("Digite o Valor de E\n");
        scanf("%lf",&E);
        setbuf(stdin,NULL);
        printf("Digite o Valor de F\n");
        scanf("%lf",&F);
        setbuf(stdin,NULL);
        printf("Digite o Valor de G\n");
        scanf("%lf",&G);
        setbuf(stdin,NULL);

        printf("y = %.1lfx^6+%.1lfx^5+%.1lf^4+%.1lfx^3+%.1lfx^2+%.1lfx+%.1lf\n",A, B, C, D, E, F, G);
        printf("Resposta:\n");
        printf("y' = 6.%.1lfx^5 + 5.%.1lfx^4 + 4.%.1lfx^3 + 3.%.1lfx^2 + 2.%.1lfx + %.1lf\n",A, B, C, D, E, F);

        Calculo = 6 * A;
        Calculo1 = 5 * B;
        Calculo2 = 4 * C;
        Calculo3 = 3 * D;
        Calculo4 = 2 * E;

        printf("y' = %.1lfx^5 + %.1lfx^4 + %.1lfx^3 + %.1lfx^2 + %.1lfx + %.1lf \n",Calculo, Calculo1, Calculo2, Calculo3, Calculo4, F);
}

void Poli7(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^7+Bx^6+Cx^5+Dx^4+Ex^3+Fx^2+Gx+H\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);
        printf("Digite o Valor de E\n");
        scanf("%lf",&E);
        setbuf(stdin,NULL);
        printf("Digite o Valor de F\n");
        scanf("%lf",&F);
        setbuf(stdin,NULL);
        printf("Digite o Valor de G\n");
        scanf("%lf",&G);
        setbuf(stdin,NULL);
        printf("Digite o Valor de H\n");
        scanf("%lf",&H);
        setbuf(stdin,NULL);


        printf("y = %.1lfx^7+%.1lfx^6+%.1lf^5+%.1lfx^4+%.1lfx^3+%.1lfx^2+%.1lfx+%.1lf \n",A, B, C, D, E, F, G, H);
        printf("Resposta:\n");
        printf("y' = 7.%.1lfx^6 + 6.%.1lfx^5 + 5.%.1lfx^4 + 4.%.1lfx^3 + 3.%.1lfx^2 + 2.%.1lfx + %.1lf\n",A, B, C, D, E, F, G);

        Calculo = 7 * A;
        Calculo1 = 6 * B;
        Calculo2 = 5 * C;
        Calculo3 = 4 * D;
        Calculo4 = 3 * E;
        Calculo5 = 2 * F;

        printf("y' = %.1lfx^6 + %.1lfx^5 + %.1lfx^4 + %.1lfx^3 + %.1lfx^2 + %.1lfx + %.1lf \n",Calculo, Calculo1, Calculo2, Calculo3, Calculo4, Calculo5, G);
}

void Poli8(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^8+Bx^7+Cx^6+Dx^5+Ex^4+Fx^3+Gx^2+Hx+I\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);
        printf("Digite o Valor de E\n");
        scanf("%lf",&E);
        setbuf(stdin,NULL);
        printf("Digite o Valor de F\n");
        scanf("%lf",&F);
        setbuf(stdin,NULL);
        printf("Digite o Valor de G\n");
        scanf("%lf",&G);
        setbuf(stdin,NULL);
        printf("Digite o Valor de H\n");
        scanf("%lf",&H);
        setbuf(stdin,NULL);
        printf("Digite o Valor de I\n");
        scanf("%lf",&I);
        setbuf(stdin,NULL);


        printf("y = %.1lfx^8+%.1lfx^7+%.1lf^6+%.1lfx^5+%.1lfx^4+%.1lfx^3+%.1lfx^2+%.1lfx+%.1lf \n",A, B, C, D, E, F, G, H, I);
        printf("Resposta:\n");
        printf("y' = 8.%.1lfx^7 + 7.%.1lfx^6 + 6.%.1lfx^5 + 5.%.1lfx^4 + 4.%.1lfx^3 + 3.%.1lfx^2 + 2.%.1lfx + %.1lf\n",A, B, C, D, E, F, G, H);

        Calculo =  8 * A;
        Calculo1 = 7 * B;
        Calculo2 = 6 * C;
        Calculo3 = 5 * D;
        Calculo4 = 4 * E;
        Calculo5 = 3 * F;
        Calculo6 = 2 * G;

        printf("y' = %.1lfx^7 + %.1lfx^6 + %.1lfx^5 + %.1lfx^4 + %.1lfx^3 + %.1lfx^2 + %.1lfx + %.1lf \n",Calculo, Calculo1, Calculo2, Calculo3, Calculo4, Calculo5, Calculo6, H);
}

void Poli9(){

        printf("Voce escolheu Derivada de Polinomio do tipo Ax^9+Bx^8+Cx^7+Dx^6+Ex^5+Fx^4+Gx^3+Hx^2+Ix+J\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);
        printf("Digite o Valor de E\n");
        scanf("%lf",&E);
        setbuf(stdin,NULL);
        printf("Digite o Valor de F\n");
        scanf("%lf",&F);
        setbuf(stdin,NULL);
        printf("Digite o Valor de G\n");
        scanf("%lf",&G);
        setbuf(stdin,NULL);
        printf("Digite o Valor de H\n");
        scanf("%lf",&H);
        setbuf(stdin,NULL);
        printf("Digite o Valor de I\n");
        scanf("%lf",&I);
        setbuf(stdin,NULL);
        printf("Digite o Valor de J\n");
        scanf("%lf",&J);
        setbuf(stdin,NULL);


        printf("y = %.1lfx^9+%.1lfx^8+%.1lf^7+%.1lfx^6+%.1lfx^5+%.1lfx^4+%.1lfx^3+%.1lfx^2+%.1lfx+%.1lf \n",A, B, C, D, E, F, G, H, I, J);
        printf("Resposta:\n");
        printf("y' = 9.%.1lfx^8 + 8.%.1lfx^7 + 7.%.1lfx^6 + 6.%.1lfx^5 + 5.%.1lfx^4 + 4.%.1lfx^3 + 3.%.1lfx^2 + 2.%.1lfx + %.1lf \n\n",A, B, C, D, E, F, G, H, I);

        Calculo =  9 * A;
        Calculo1 = 8 * B;
        Calculo2 = 7 * C;
        Calculo3 = 6 * D;
        Calculo4 = 5 * E;
        Calculo5 = 4 * F;
        Calculo6 = 3 * G;
        Calculo7 = 2 * H;

        printf("y' = %.1lfx^8 + %.1lfx^7 + %.1lfx^6 + %.1lfx^5 + %.1lfx^4 + %.1lfx^3 + %.1lfx^2 + %.1lfx + %.1lf \n",Calculo, Calculo1, Calculo2, Calculo3, Calculo4, Calculo5, Calculo6, Calculo7, I);




}

void Poli10(){


        printf("Voce escolheu Derivada de Polinomio do tipo Ax^10+Bx^9+Cx^8+Dx^7+Ex^6+Fx^5+Gx^4+Hx^3+Ix^2+Jx+K\n");
        printf("Digite o Valor de A\n");
        scanf("%lf",&A);
        setbuf(stdin,NULL);
        printf("Digite o Valor de B\n");
        scanf("%lf",&B);
        setbuf(stdin,NULL);
        printf("Digite o Valor de C\n");
        scanf("%lf",&C);
        setbuf(stdin,NULL);
        printf("Digite o Valor de D\n");
        scanf("%lf",&D);
        setbuf(stdin,NULL);
        printf("Digite o Valor de E\n");
        scanf("%lf",&E);
        setbuf(stdin,NULL);
        printf("Digite o Valor de F\n");
        scanf("%lf",&F);
        setbuf(stdin,NULL);
        printf("Digite o Valor de G\n");
        scanf("%lf",&G);
        setbuf(stdin,NULL);
        printf("Digite o Valor de H\n");
        scanf("%lf",&H);
        setbuf(stdin,NULL);
        printf("Digite o Valor de I\n");
        scanf("%lf",&I);
        setbuf(stdin,NULL);
        printf("Digite o Valor de J\n");
        scanf("%lf",&J);
        setbuf(stdin,NULL);
        printf("Digite o Valor de K\n");
        scanf("%lf",&K);
        setbuf(stdin,NULL);


        printf("y = %.1lfx^10+%.1lfx^9+%.1lf^8+%.1lfx^7+%.1lfx^6+%.1lfx^5+%.1lfx^4+%.1lfx^3+%.1lfx^2+%.1lfx+%.1lf \n",A, B, C, D, E, F, G, H, I, J, K);
        printf("Resposta:\n");
        printf("y' = 10.%.1lfx^9 + 9.%.1lfx^8 + 8.%.1lfx^7 + 7.%.1lfx^6 + 6.%.1lfx^5 + 5.%.1lfx^4 + 4.%.1lfx^3 + 3.%.1lfx^2 + 2.%.1lfx + %.1lf  \n",A, B, C, D, E, F, G, H, I, J);

        Calculo =  10 * A;
        Calculo1 = 9 * B;
        Calculo2 = 8 * C;
        Calculo3 = 7 * D;
        Calculo4 = 6 * E;
        Calculo5 = 5 * F;
        Calculo6 = 4 * G;
        Calculo7 = 3 * H;
        Calculo8 = 2 * I;

        printf("y' = %.1lfx^8 + %.1lfx^7 + %.1lfx^6 + %.1lfx^5 + %.1lfx^4 + %.1lfx^3 + %.1lfx^2 + %.1lfx + %.1lf \n",Calculo, Calculo1, Calculo2, Calculo3, Calculo4, Calculo5, Calculo6, Calculo7, Calculo8, J);


}

void LNU(){

    printf("________________________________________________________________________________\n");

    printf("Você escolheu derivada de funcao do tipo Ln(U)\n");

    printf("Escolha qual tipo de funcao se deseja usar como U\n");
    printf("1- Funcão Trigonometrica         2- Funcão Polinomial de 1 grau \n");

    scanf("%d",&number);
    setbuf(stdin,NULL);
    printf("________________________________________________________________________________\n");

    switch(number){

    case 1:

        printf("Digite o valor de U\n");
        scanf("%[^\n]c",&U);
        setbuf(stdin,NULL);
        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6]){

        printf("y= ln(sin(x))\n\n");

        // Fazendo pela regra da cadeia f= lnU e u = sinx

        printf("y= d/du (ln(u)) d/dx (sin(x)) \n\n ");

        printf("d/du ln(u) = 1/u\ e d/dx (sin(x)) = cos(x) n\n");

        printf("y = 1/u.cos(x)\n\n");

        // voltando u = sinx

        printf("y'= 1.cos(x)/sin(x)\n\n");

        //simplificando

        printf("y'= cot(x)\n\n");

        }else

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5]){

        printf("y= ln(cos(x))\n\n");

        //regra da cadeia lnu e u = cosx

        printf("y= d/du ln(u) d/dx cos(x)\n\n");

        printf("d/du ln(u) = 1/u e d/dx (cos(x)) = -sin(x)\n\n");

        printf("y'= 1.(-sin(x))/u\n\n");

        //voltando u = cosx

        printf("y'= -sin(x)/cos(x)\n\n");

        printf("y'= - tg(x)\n\n");


        }else

        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5]){

         printf("y= ln(tg(x))\n\n");

        // regra da cadeia lnu e u = tg(x)

        printf("y= d/du ln(u) d/dx tg(x)\n\n");

        printf("d/du ln(u) = 1/u e d/dx (tg(x)) = sec^2(x)\n\n");

        printf("y= 1.sec^2(x)/u\n\n");

        // voltando u = tgx

        printf("y'= sec^2/tg(x)\n\n");

        printf("y'= 2cossec(2x)\n\n");

        }

    case 2:

        printf("Digite o valor de U para a funcao ln(Ux^K)\n\n");
        scanf("%lf",&U1);

        printf("Digite o valor de K para a funcao ln(Ux^K)\n\n");
        scanf("%lf",&U2);

        printf("\n\n");

        printf("y= ln(%.1lfx^%.1lf\n\n",U1 ,U2);

        // regra da cadeia f = lnu u= ux^k

        printf("y= d/du (ln(u)) d/dx (%.1lfx^%.1lf)\n\n", U1, U2);

        Conta1 = U2 * U1;
        Conta2 = U2 - 1;

        printf("d/du ln(u) = 1/u e d/dx (%.1lfx^%.1lf) = %.1lfx^%.1lf \n\n",U1 ,U2, Conta1, Conta2);

        printf("y= 1/u . %.1lfx^%.1lf\n\n", Conta1, Conta2);

        // voltando u =valor

        printf("y'= 1/(%.1lfx^%.1lf) . %.1lfx^%.1lf\n\n", U1, U2, Conta1, Conta2);

        printf("y'= %.1lf/x\n\n",U2);







    }





}

void UN(){

        printf("Voce escolheu de funcao do tipo u^N (Com N pertencendo aos reais) \n");
        printf("Digite o Valor de N\n");
        scanf("%lf",&N);
        setbuf(stdin,NULL);

        printf("y = x^%.1lf\n",N);
        printf("Resposta:\n");



        Z = N - 1;


        printf("y' = %.1lf.x^%.1lf\n",N , Z);

}

void UV(){

    printf("________________________________________________________________________________\n");

    printf("Você escolheu derivada de funcao do tipo U.V\n");

    printf("Escolha qual tipo de funcao se deseja usar como U.V\n");
    printf("1- Funcão Trigonometrica         2- Funcao Exponencial \n");
    printf("3- Funcão Mista(Trigonometrica e Exponencial)\n");


    scanf("%d",&number);
    setbuf(stdin,NULL);
    printf("________________________________________________________________________________\n");

    switch(number){

    case 1:

        printf("Digite o valor de U\n");
        scanf("%[^\n]c",&U);
        setbuf(stdin,NULL);

        printf("Digite o valor de V\n");
        scanf("%[^\n]c",&V);
        setbuf(stdin,NULL);

        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6] && V[0]==F0[0] && V[1]==F0[1] && V[2]==F0[2] && V[3]==F0[3] && V[4]==F0[4] && V[5]==F0[5] && V[6]==F0[6]){

        printf("y = sin^2(x)\n\n");

        //Regra da cadeia f=u^2 e u=sinx

        printf("d/du (u^2) d/dx sin(x)\n\n");

        printf("d/du (u^2) = 2u e d/dx sin(x) = cos(x)\n\n");

        printf("y = 2u.cos(x)\n\n");

        //voltando u

        printf("y'= 2.sin(x).cos(x)\n\n");

        printf("y'= sin(2x)\n\n"); // propriedade trigonometrica da tabela de derivadas utilizada.

        }else

        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6] && V[0]==F1[0] && V[1]==F1[1] && V[2]==F1[2] && V[3]==F1[3] && V[4]==F1[4] && V[5]==F1[5] ){


        printf("sin(x).cos(x)\n\n");

        // regra do produto f = sinx e g = cosx

        printf("d/dx (sin(x)).cos(x) + d/dx (cos(x)).sin(x)\n\n");

        printf("d/dx (sin(x)) = cos(x) e d/dx (cos(x)) = -sin(x)\n\n");

        printf("y'= cos(x).cos(x) + (-sin(x)).sin(x)\n\n");

        printf("y'= cos(2x)\n\n");


        }else

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5] && V[0]==F0[0] && V[1]==F0[1] && V[2]==F0[2] && V[3]==F0[3] && V[4]==F0[4] && V[5]==F0[5] && U[6]==F0[6]){


        printf("cos(x).sin(x)\n\n");

        // regra do produto f = sinx e g = cosx

        printf("d/dx (sin(x)).cos(x) + d/dx (cos(x)).sin(x)\n\n");

        printf("d/dx (sin(x)) = cos(x) e d/dx (cos(x)) = -sin(x)\n\n");

        printf("y'= cos(x).cos(x) + (-sin(x)).sin(x)\n\n");

        printf("y'= cos(2x)\n\n");


        }else

        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6] && V[0]==F2[0] && V[1]==F2[1] && V[2]==F2[2] && V[3]==F2[3] && V[4]==F2[4] && V[5]==F2[5]){

        printf("sin(x).tg(x)\n\n");

        //regra do produto

        printf("d/dx (sin(x)).tg(x) + d/dx (tg(x)).sin(x)\n\n");

        printf("d/dx (sin(x)) = cos(x) e d/dx tg(x) = sec^2(x)\n\n");

        printf("y' = cos(x).tg(x) + sec^2(x).sin(x)\n\n");

        printf("y' = sin(x).(1+sec^2(x))\n\n");


        }else

        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5] && V[0]==F0[0] && V[1]==F0[1] && V[2]==F0[2] && V[3]==F0[3] && V[4]==F0[4] && V[5]==F0[5] && V[6]==F0[6]){

        printf("tg(x).sin(x)\n\n");

        //regra do produto

        printf("d/dx (sin(x)).tg(x) + d/dx (tg(x)).sin(x)\n\n");

        printf("d/dx (sin(x)) = cos(x) e d/dx tg(x) = sec^2(x)\n\n");

        printf("y' = cos(x).tg(x) + sec^2(x).sin(x)\n\n");

        printf("y' = sin(x).(1+sec^2(x))\n\n");


        }else

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5] && V[0]==F2[0] && V[1]==F2[1] && V[2]==F2[2] && V[3]==F2[3] && V[4]==F2[4] && V[5]==F2[5]){

            printf("y= cos(x).tg(x)\n\n");

            // usando a propriedade trigonometrica tg = sin/cos

            printf("y= sin(x)\n\n");

            printf("d/dx sin(x)\n\n");

            printf("y'= cos(x)\n\n");

            }else

        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5] && V[0]==F1[0] && V[1]==F1[1] && V[2]==F1[2] && V[3]==F1[3] && V[4]==F1[4] && V[5]==F1[5]){

            printf("y= cos(x).tg(x)\n\n");

            // usando a propriedade trigonometrica tg = sin/cos

            printf("y= sin(x)\n\n");

            printf("d/dx sin(x)\n\n");

            printf("y'= cos(x)\n\n");

            }else



        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5] && V[0]==F1[0] && V[1]==F1[1] && V[2]==F1[2] && V[3]==F1[3] && V[4]==F1[4] && V[5]==F1[5]){

            printf("y= cos^2(x)\n\n");

            //regra da cadeia f=u^2 e u=cos(x)

            printf("d/du (u^2) = 2u e d/dx (cos(x)) = -sin(x)\n\n");

            printf("y= 2u(-sin(x))\n\n");

            printf("y'= 2cos(x).(-sin(x))\n\n");

            printf("y'= -sin(2x)\n\n");

            }else

         if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5] && V[0]==F2[0] && V[1]==F2[1] && V[2]==F2[2] && V[3]==F2[3] && V[4]==F2[4] && V[5]==F2[5]){

            printf("y= tg^2(x)\n\n");

            //regra da cadeia

            printf("d/du (u^2) e d/dx tg(x)\n\n");

            printf("d/du (u^2) = 2u e d/dx tg(x) = sec^2(x)\n\n");

            printf("y= 2.u.sec^2(x)\n\n");

            printf("y'= 2tg(x).sec^2(x)\n\n");

            }

        break;

    case 2:


        printf("Digite o valor de U para a funcao (Ux^K . Zx^W)\n\n");
        scanf("%lf",&U1);

        printf("Digite o valor de K para a funcao (Ux^K . Zx^W)\n\n");
        scanf("%lf",&U2);

        printf("Digite o valor de Z para a funcao (Ux^K . Zx^W)\n\n");
        scanf("%lf",&U3);

        printf("Digite o valor de W para a funcao (Ux^K . Zx^W)\n\n");
        scanf("%lf",&U4);


        printf("\n\n");

        printf("y= %.1lfx^%.1lf . %.1lfx^%.1lf\n\n",U1,U2,U3,U4);

        Conta1 = U1 * U3;

        printf("%.1lf d/dx (x^%.1lf.x^%.1lf)\n\n",Conta1,U2,U4);

        // regra do produto

        printf("%.1lf[ d/dx (x^%.1lf).(x^%.1lf) + d/dx(x^%.1lf).(x^%.1lf)\n\n",Conta1,U2,U4,U4,U2);

        Conta2 = U2 - 1;

        Conta3 = U4 - 1;

        printf("d/dx (x^%.1lf) = %.1lfx^%.1lf e d/dx (x^%.1lf) = %.1lfx^%.1lf \n\n",U2,U2,Conta2,U4,U4,Conta3);

        printf("y= %.1lf(%.1lfx^%.1lfx^%.1lf + %.1lfx^%.1lfx^%.1lf\n\n)",Conta1,U2,Conta2,U4,U4,Conta3,U2);

        Conta4 = Conta3 + U2;

        Conta5 = U2 + U4;

        Conta6 = Conta5 * Conta1;


        printf("y'= %.1lfx^%.1lf\n\n",Conta6,Conta4);


    case 3:

        printf("Digite o valor de U para a funcao (Ux^K . g(x)\n\n");
        scanf("%lf",&U1);
        setbuf(stdin,NULL);

        printf("Digite o valor de U para a funcao (Ux^K . g(x)\n\n");
        scanf("%lf",&U2);
        setbuf(stdin,NULL);

        printf("Digite o valor de g(x)\n\n");
        scanf("%[^\n]c",&U);
        setbuf(stdin,NULL);

        printf("\n\n");

        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6]){

            printf("%.1lfx^%.1lf . sin(x)\n\n",U1,U2);

            printf("%.1lf d/dx (x^%.1lf . sin(x)\n\n",U1,U2);

            //regra do produto f = x^7 e g = sin(x)

            printf("%.1lf(d/dx (x^%.1lf).sin(x) + d/dx (sin(x)). x^%.1lf",U1,U2,U2);

            Conta1 = U2 - 1;

            printf("d/dx (x^%.1lf) = %.1lfx^%.1lf e d/dx sin(x) = cos(x)\n\n",U2,U2,Conta1);

            printf("y'= %.1lf(%.1lfx^%.1lf.sin(x) + cos(x).x^%.1lf\n\n",U1,U2,Conta1,U2);
            }

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5]){


            printf("%.1lfx^%.1lf . cos(x)\n\n",U1,U2);

            printf("%.1lf d/dx (x^%.1lf . cos(x)\n\n",U1,U2);

             //regra do produto

            printf("%.1lf(d/dx (x^%.1lf).cos(x) + d/dx (cos(x)). x^%.1lf\n\n",U1,U2,U2);

            Conta1 = U2 - 1;

            printf("d/dx (x^%.1lf) = %.1lfx^%.1lf e d/dx cos(x) = -sin(x)\n\n",U2,U2,Conta1);

            printf("y'= %.1lf(%.1lfx^%.1lf . cos(x) - x^%.1lf . sin(x) \n\n",U1,U2,Conta1,U2);

        }

        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5]){



            printf("%.1lfx^%.1lf . tg(x)\n\n",U1,U2);

            printf("%.1lf d/dx (x^%.1lf . tg(x)\n\n",U1,U2);

            //regra do produto

            printf("%.1lf(d/dx (x^%.1lf).tg(x) + d/dx (tg(x)). x^%.1lf\n\n",U1,U2,U2);

            Conta1 = U2 - 1;

            printf("d/dx (x^%.1lf) = %.1lfx^%.1lf e d/dx tg(x) = sec^2(x)\n\n",U2,U2,Conta1);

            printf("y'= %.1lf(%.1lfx^%.1lf . tg(x) + x^%.1lf . sec^2(x) \n\n",U1,U2,Conta1,U2);











        }





    }



}

void UV2(){

    printf("________________________________________________________________________________\n");

    printf("Você escolheu derivada de funcao do tipo U/V\n\n");

    printf("Escolha qual tipo de funcao se deseja usar como U/V\n");
    printf("1- Funcão Trigonometrica         2- Funcao Exponencial \n");
    printf("3- Funcão Mista trigo/expo       4- Funcao Mista expo/trigo\n");


    scanf("%d",&number);
    setbuf(stdin,NULL);
    printf("________________________________________________________________________________\n");

     switch(number){

    case 1:

        printf("Digite o valor de U\n");
        scanf("%[^\n]c",&U);
        setbuf(stdin,NULL);

        printf("Digite o valor de V\n");
        scanf("%[^\n]c",&V);
        setbuf(stdin,NULL);

        printf("\n\n");

       if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6] && V[0]==F0[0] && V[1]==F0[1] && V[2]==F0[2] && V[3]==F0[3] && V[4]==F0[4] && V[5]==F0[5] && V[6]==F0[6]){

            printf("y= sin(x)/sin(x)\n\n");

            printf("y= 1\n\n");

            printf("y'= 0\n\n");

    }

         if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6] && V[0]==F1[0] && V[1]==F1[1] && V[2]==F1[2] && V[3]==F1[3] && V[4]==F1[4] && V[5]==F1[5] ){

            printf("y= sin(x)/cos(x)\n\n");

            printf("y = tg(x)\n\n");

            printf("y'= sec^2(x)\n\n");


    }

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5] && V[0]==F0[0] && V[1]==F0[1] && V[2]==F0[2] && V[3]==F0[3] && V[4]==F0[4] && V[5]==F0[5] && U[6]==F0[6]){

            printf("y= cos(x)/sin(x)\n\n");

            printf("y= cotg(x)\n\n");

            printf("y'= - cossec^2(x)\n\n");



    }

        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6] && V[0]==F2[0] && V[1]==F2[1] && V[2]==F2[2] && V[3]==F2[3] && V[4]==F2[4] && V[5]==F2[5]){

            printf("y= sin(x)/tg(x)\n\n");

            printf("y= cos(x)\n\n");

            printf("y'= -sin(x)\n\n");



    }


        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5] && V[0]==F0[0] && V[1]==F0[1] && V[2]==F0[2] && V[3]==F0[3] && V[4]==F0[4] && V[5]==F0[5] && V[6]==F0[6]){

            printf("tg(x)/sin(x)\n\n");

        // regra do quociente

            printf("[d/dx (tg(x)).sin(x) - d/dx (sin(x)).tg(x)] / (sin(x))^2\n\n");

            printf("d/dx tg(x) = sec^2(x) e d/dx sin(x) = cos(x) \n\n");

            printf("y'= [sec^2(x). sin(x) - cos(x). tg(x)] / (sin(x))^2 \n\n");

            printf("y'= [sec(x).tg(x) - sin(x)] / sin^2(x) \n\n");

    }

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5] && V[0]==F2[0] && V[1]==F2[1] && V[2]==F2[2] && V[3]==F2[3] && V[4]==F2[4] && V[5]==F2[5]){

            printf("y= cos(x)/tg(x)\n\n");

            //regra do quociente

            printf("y= [d/dx(cos(x)).tg(x) - d/dx tg(x).cos(x)] / (tg(x)^2)\n\n");

            printf("d/dx cos(x) = -sin(x) e d/dx tg(x) = sec^2(x)\n\n");

            printf("y'= [-sin(x). tg(x) - sec^2(x).cos(x)] / (tg(x))^2\n\n");

            printf("y'= -sin(x).tg(x) - sec^2(x).cos(x) / tg^2(x)\n\n");

    }


        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5] && V[0]==F1[0] && V[1]==F1[1] && V[2]==F1[2] && V[3]==F1[3] && V[4]==F1[4] && V[5]==F1[5]){

            printf("y= cos(x)/cos(x)\n\n");

            printf("y= 1\n\n");

            printf("y' = 0\n\n");


        }


        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5] && V[0]==F2[0] && V[1]==F2[1] && V[2]==F2[2] && V[3]==F2[3] && V[4]==F2[4] && V[5]==F2[5]){

            printf("y= tg(x)/tg(x)\n\n");

            printf("y= 1\n\n");

            printf("y' = 0\n\n");


    }


    case 2:

        printf("Digite o valor de U para a funcao (Ux^K / Zx^W)\n\n");
        scanf("%lf",&U1);

        printf("Digite o valor de K para a funcao (Ux^K / Zx^W)\n\n");
        scanf("%lf",&U2);

        printf("Digite o valor de Z para a funcao (Ux^K / Zx^W)\n\n");
        scanf("%lf",&U3);

        printf("Digite o valor de W para a funcao (Ux^K / Zx^W)\n\n");
        scanf("%lf",&U4);

        printf("\n\n");

        printf("y= %.1lfx^%.1lf / %.1lfx^%.1lf\n\n",U1,U2,U3,U4);

        printf("y= %.1lf / %.1lf d/dx (x^%.1lf / x^%.1lf\n\n",U1,U3,U2,U4);

        //regra do quociente

        printf("%.1lf/%.1lf . [d/dx (x^%.1lf).x^%.1lf - d/dx (x^%.1lf).x^%.1lf ] / (x^%.1lf)^2 \n\n",U1,U3,U2,U4,U4,U2,U4);

        Conta1 = U2 - 1;
        Conta2 = U4 - 1;

        printf("d/dx x^%.1lf = %.1lfx^%.1lf e d/dx x^%.1lf = %.1lfx^%.1lf \n\n",U2,U2,Conta1,U4,U4,Conta2);

        printf("y= %.1lf/%.1lf . %.1lfx^%.1lf . x^%.1lf - %.1lfx^%.1lf . x^%.1lf / (x^%.1lf)^2\n\n",U1,U3,U2,Conta1,U4,U4,Conta2,U2,U4);



        Conta3 = U2 - U4; // 4

        Conta4 = (U4 * 2); // 6

        Conta5 = (Conta1 + U4); // 6 + 3 = 9

        Conta6 = Conta5 - Conta4; // = 3





        printf("%.1lf/%.1lf . %.1lfx^%.1lf / x^%.1lf \n\n",U1,U3,Conta3,Conta6,Conta5);

        Conta7 = Conta3 * U1;

        printf("%.1lfx^%.1lf / %.1lf\n\n",Conta7,Conta6,U3);


    case 3:

        printf("Você escolheu a funcao do tipo trigo/expo (U/V) \n\n");

        printf("Digite o valor de U\n"); // trigo
        scanf("%[^\n]c",&U);
        setbuf(stdin,NULL);

        printf("Digite o valor de K para Kx^V\n\n");
        scanf("%lf",&U2);
        setbuf(stdin,NULL);
        printf("Digite o valor de V para Kx^v\n\n");
        scanf("%lf",&U3);
        setbuf(stdin,NULL);

        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6]){

        printf("y= sin(x)/%.1lfx^%.1lf\n\n",U2,U3);

        printf("y= 1/%.1lf . d/dx . (sin(x)/x^%.1lf\n\n",U2,U3);

        printf("y= 1/%.1lf . d/dx [sin(x)x^%.1lf - d/dx x^%.1lf.sin(x)] / (x^%.1lf)^2\n\n",U2,U3,U3,U3); // errada

        Conta1 = U3 - 1;

        printf("d/dx sin(x) = cos(x) e d/dx x^%.1lf = %.1lfx^%.1lf \n\n",U3,U3,Conta1);

        printf("y= 1/%.1lf . [cos(x)x^%.1lf - %.1lfx^%.1lf.sin(x)] / (x^%.1lf)^2\n\n",U2,U3,U3,Conta1,U2);

        Conta2 = U3 * 2;

        Conta3 = Conta2 - Conta1;


        printf("[x.cos(x) - %.1lf.sin(x)] / %.1lfx^%.1lf\n\n",U3,U2,Conta3);



    }

         if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5]){


            printf("y= cos(x)/%.1lfx^%.1lf\n\n",U2,U3);

            printf("y= 1/%.1lf . d/dx . (cos(x)/x^%.1lf\n\n",U2,U3);

            printf("y= 1/%.1lf . d/dx [cos(x)x^%.1lf - d/dx x^%.1lf.cos(x)] / (x^%.1lf)^2\n\n",U2,U3,U3,U3);

            Conta1 = U3 - 1;

            printf("d/dx cos(x) = -sin(x) e d/dx x^%.1lf = %.1lfx^%.1lf \n\n",U3,U3,Conta1);

            printf("y= 1/%.1lf . [-sin(x)x^%.1lf - %.1lfx^%.1lf.cos(x)] / (x^%.1lf)^2\n\n",U2,U3,U3,Conta1,U2);

            Conta2 = U3 * 2;

            Conta3 = Conta2 - Conta1;

            printf("[- x.sin(x) + %.1lf.cos(x)] / %.1lfx^%.1lf\n\n",U3,U2,Conta3);


    }

            if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5]){

            printf("y= tg(x)/%.1lfx^%.1lf\n\n",U2,U3);

            printf("y= 1/%.1lf . d/dx . (tg(x))/x^%.1lf\n\n",U2,U3);

            printf("y= 1/%.1lf . d/dx [tg(x)x^%.1lf - d/dx x^%.1lf.tg(x)] / (x^%.1lf)^2\n\n",U2,U3,U3,U3);

            Conta1 = U3 - 1;

            printf("d/dx tg(x) = sec^2(x) e d/dx x^%.1lf = %.1lfx^%.1lf \n\n",U3,U3,Conta1);

            printf("y= 1/%.1lf . [sec^2(x).x^%.1lf - %.1lfx^%.1lf.tg(x)] / (x^%.1lf)^2\n\n",U2,U3,U3,Conta1,U3);


            Conta2 = U3 * 2;

            Conta3 = Conta2 - Conta1;

            printf("[x.sec^2(x) - %.1lf.tg(x)] / %.1lfx^%.1lf\n\n",U3,U2,Conta3);



    }


    case 4: //4- Funcao Mista expo/trigo\n");



            printf("Você escolheu a funcao do tipo expo/trigo (U/V) \n\n");

            printf("Digite o valor de K para Kx^V\n\n");
            scanf("%lf",&U2);
            setbuf(stdin,NULL);
            printf("Digite o valor de V para Kx^v\n\n");
            scanf("%lf",&U3);
            setbuf(stdin,NULL);

            printf("Digite o valor de U\n"); // trigo
            scanf("%[^\n]c",&U);
            setbuf(stdin,NULL);

             if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6]){

                    printf("y= %.1lfx^%.1lf / sin(x)\n\n",U2,U3);

                    printf("%.1lf d/dx (x^%.1lf/ sin(x)\n\n",U2,U3);

                    // regra do quociente

                    printf("y= %.1lf . [d/dx(x^%.1lf).sin(x) - d/dx (sin(x)) . x^%.1lf] / (sin(x))^2\n\n",U2,U3,U3);

                    Conta1 = U3 - 1;

                    printf("d/dx (x^%.1lf) = %.1lfx^%.1lf e d/dx (sin(x) = cos(x)\n\n",U3,U3,Conta1);

                    printf("y'= %.1lf.[%.1lfx^%.1lf.sin(x) - x^%.1lf.cos(x)] / sin^2(x)\n\n",U2,U3,Conta1,U3);








     }


}

}

void EU(){

    printf("________________________________________________________________________________\n");

        printf("Voce escolheu a funcao do tipo e^U\n");

        printf("Escolha o que deseja usar como U\n\n");

        printf("1- Funcão Trigonometrica         2- Funcão Polinomial de 1 grau \n");

        scanf("%d",&Func);
        setbuf(stdin,NULL);
        printf("________________________________________________________________________________\n");


        switch(Func){

        case 1:

        printf("Digite o valor de U\n");
        scanf("%[^\n]c",&U);
        setbuf(stdin,NULL);
        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6]){

            printf("e^sin(x)\n");


            printf("e^sin(x) . cos(x)\n");

        }else

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5] && U[6]==F1[6]){

            printf("e^cos(x)\n");


            printf(" - e^cos(x) . sin(x) \n");


        }else



        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5]){

            printf("e^tg(x)\n");


            printf("e^tg(x) . sec^2(x)\n");


        }

        break;

        case 2:

        printf("Digite o valor de U na expressao e^Ux\n");
        scanf("%lf",&U1);
        setbuf(stdin,NULL);
        printf("e^%.1lfx\n",U1);

        printf("resposta\n");

        printf("%.1lfe^%.1lfx\n",U1,U1);



        break;


        }

}

void SINU(){

    printf("Voce escolheu derivada de funcao do tipo sin(ux^k)\n\n");

    printf("Digite o valor de u para a funcao ux^k\n");
    scanf("%lf",&U1);
    setbuf(stdin,NULL);

    printf("Digite o valor de k para a funcao ux^k\n");
    scanf("%lf",&U2);
    setbuf(stdin,NULL);

    if(U1 == 1 && U2 == 1){

        printf("cos(x)\n\n");

    }else{

        printf("y= sin(%.1lfx^%.1lf)\n\n",U1,U2);

        // regra da cadeia f=sin(u) e u= %.1lfx^%.1lf

        printf("y= d/du sin(u) . d/dx (%.1lfx^%.1lf)\n\n",U1,U2);

        Conta1 = U1 * U2;
        Conta2 = U2 - 1;

        printf("d/du sin(u) = cos(u) e d/dx (%.1lfx^%.1lf) = %.1lfx^%.1lf\n\n",U1,U2,Conta1,Conta2);

        printf("y'= cos(u) . %.1lfx^%.1lf\n\n",Conta1,Conta2);

        printf("y'= cos(%.1lfx^%.1lf) . %.1lfx^%.1lf \n\n",U1,U2,Conta1,Conta2);







    }

}

void COSU(){

    printf("Você escolheu derivada de funcao do tipo cos(ux^k)\n\n");

    printf("Digite o valor de u para a função ux^k\n");
    scanf("%lf",&U1);
    setbuf(stdin,NULL);

    printf("Digite o valor de k para a função ux^k\n");
    scanf("%lf",&U2);
    setbuf(stdin,NULL);

    if(U1 == 1 && U2 == 1){

        printf("-sin(x)\n\n");

    }else{

        printf("y= cos(%.1lfx^%.1lf)\n\n",U1,U2);

        // regra da cadeia f=cos(u) e u= %.1lfx^%.1lf

        printf("y= d/du cos(u) . d/dx (%.1lfx^%.1lf)\n\n",U1,U2);

        Conta1 = U1 * U2;
        Conta2 = U2 - 1;

        printf("d/du sin(u) = -sin(u) e d/dx (%.1lfx^%.1lf) = %.1lfx^%.1lf\n\n",U1,U2,Conta1,Conta2);

        printf("y'= -sin(u) . %.1lfx^%.1lf\n\n",Conta1,Conta2);

        printf("y'= -sin(%.1lfx^%.1lf) . %.1lfx^%.1lf \n\n",U1,U2,Conta1,Conta2);
    }

}

void TGU(){

    printf("Você escolheu derivada de funcao do tipo tg(ux^k)\n\n");

    printf("Digite o valor de u para a função ux^k\n");
    scanf("%lf",&U1);
    setbuf(stdin,NULL);

    printf("Digite o valor de k para a função ux^k\n");
    scanf("%lf",&U2);
    setbuf(stdin,NULL);

    if(U1 == 1 && U2 == 1){

        printf("sec^2(x)\n\n");

    }else{

        printf("y= tg(%.1lfx^%.1lf)\n\n",U1,U2);

        // regra da cadeia f=cos(u) e u= %.1lfx^%.1lf

        printf("y= d/du tg(u) . d/dx (%.1lfx^%.1lf)\n\n",U1,U2);

        Conta1 = U1 * U2;
        Conta2 = U2 - 1;

        printf("d/du tg(u) = sec^2(u) e d/dx (%.1lfx^%.1lf) = %.1lfx^%.1lf\n\n",U1,U2,Conta1,Conta2);

        printf("y'= sec^2(u) . %.1lfx^%.1lf\n\n",Conta1,Conta2);

        printf("y'= sec^2(%.1lfx^%.1lf) . %.1lfx^%.1lf \n\n",U1,U2,Conta1,Conta2);

    }

}

void SECU(){

     printf("Você escolheu derivada de funcao do tipo sec(ux^k)\n\n");

    printf("Digite o valor de u para a função ux^k\n");
    scanf("%lf",&U1);
    setbuf(stdin,NULL);

    printf("Digite o valor de k para a função ux^k\n");
    scanf("%lf",&U2);
    setbuf(stdin,NULL);

    if(U1 == 1 && U2 == 1){

        printf("sec(x).tg(x)\n\n");

    }else{

        printf("y= sec(%.1lfx^%.1lf)\n\n",U1,U2);

        // regra da cadeia f=cos(u) e u= %.1lfx^%.1lf

        printf("y= d/du sec(u) . d/dx (%.1lfx^%.1lf)\n\n",U1,U2);

        Conta1 = U1 * U2;
        Conta2 = U2 - 1;

        printf("d/du sec(u) = sec(u).tg(u) e d/dx (%.1lfx^%.1lf) = %.1lfx^%.1lf\n\n",U1,U2,Conta1,Conta2);

        printf("y'= sec(u).tg(u) . %.1lfx^%.1lf\n\n",Conta1,Conta2);

        printf("y'= sec(%.1lfx^%.1lf).tg(%.1lfx^%.1lf) . %.1lfx^%.1lf \n\n",U1,U2,U1,U2,Conta1,Conta2);

    }

}

void COSSECU(){

printf("Você escolheu derivada de funcao do tipo cossec(ux^k)\n\n");

    printf("Digite o valor de u para a função ux^k\n");
    scanf("%lf",&U1);
    setbuf(stdin,NULL);

    printf("Digite o valor de k para a função ux^k\n");
    scanf("%lf",&U2);
    setbuf(stdin,NULL);

    if(U1 == 1 && U2 == 1){

        printf("-cotg(x).cossec(x)\n\n");

    }else{

        printf("y= cossec(%.1lfx^%.1lf)\n\n",U1,U2);

        // regra da cadeia f=cos(u) e u= %.1lfx^%.1lf

        printf("y= d/du cossec(u) . d/dx (%.1lfx^%.1lf)\n\n",U1,U2);

        Conta1 = U1 * U2;
        Conta2 = U2 - 1;

        printf("d/du cossec(u) = -cotg(u).cossec(u) e d/dx (%.1lfx^%.1lf) = %.1lfx^%.1lf\n\n",U1,U2,Conta1,Conta2);

        printf("y'= -cotg(u).cossec(u) . %.1lfx^%.1lf\n\n",Conta1,Conta2);

        printf("y'= -cotg(%.1lfx^%.1lf).cossec(%.1lfx^%.1lf) . %.1lfx^%.1lf \n\n",U1,U2,U1,U2,Conta1,Conta2);


    }

}

void COTGU(){

    printf("Você escolheu derivada de funcao do tipo cotg(ux^k)\n\n");

    printf("Digite o valor de u para a função ux^k\n");
    scanf("%lf",&U1);
    setbuf(stdin,NULL);

    printf("Digite o valor de k para a função ux^k\n");
    scanf("%lf",&U2);
    setbuf(stdin,NULL);

    if(U1 == 1 && U2 == 1){

        printf("-cossec^2(x)\n\n");

    }else{

        printf("y= cotg(%.1lfx^%.1lf)\n\n",U1,U2);

        // regra da cadeia f=cos(u) e u= %.1lfx^%.1lf

        printf("y= d/du cotg(u) . d/dx (%.1lfx^%.1lf)\n\n",U1,U2);

        Conta1 = U1 * U2;
        Conta2 = U2 - 1;

        printf("d/du cotg(u) = -cossec^2(u) e d/dx (%.1lfx^%.1lf) = %.1lfx^%.1lf\n\n",U1,U2,Conta1,Conta2);

        printf("y'= -cossec^2(u) . %.1lfx^%.1lf\n\n",Conta1,Conta2);

        printf("y'= -cossec^2(%.1lfx^%.1lf) . %.1lfx^%.1lf \n\n",U1,U2,Conta1,Conta2);







    }





}

void UV3(){

printf("________________________________________________________________________________\n");

    printf("Você escolheu derivada de funcao do tipo u^v\n");

    printf("Escolha qual tipo de funcao se deseja usar como U\n");
    printf("1- Funcão Trigonometrica         2- Funcão Polinomial\n");

    scanf("%d",&number);
    setbuf(stdin,NULL);
    printf("________________________________________________________________________________\n");


    switch(number){

    case 1:

        printf("Digite o valor de V\n");
        scanf("%[^\n]c",&U);
        setbuf(stdin,NULL);
        if(U[0]==F0[0] && U[1]==F0[1] && U[2]==F0[2] && U[3]==F0[3] && U[4]==F0[4] && U[5]==F0[5] && U[6]==F0[6]){


        printf("y= x^sin(x)\n\n");

        printf("y = d/dx x^sin(x)\n\n");

        //regra do expoente

        printf("y= (e^(sin(x).ln(x)\n\n");

        // regra da cadeia f = e^u e u = sinxlnx

        printf("y= d/du (e^u) d/dx (sin(x).ln(x))\n\n");

        printf("d/du(e^u) = e^u e d/dx (sin(x).ln(x)) = cos(x).ln(x) + sin(x)/x\n\n ");

        printf("y= e^u(cos(x).ln(x)+(sin(x)/x))\n\n");

        //voltando u

        printf("y'= e^(sin(x).ln(x)) . (cos(x).ln(x) + (sin(x)/x))\n\n");

        printf("y'= x^sin(x).[cos(x).ln(x) + (sin(x)/x)\n\n");

        }else

        if(U[0]==F1[0] && U[1]==F1[1] && U[2]==F1[2] && U[3]==F1[3] && U[4]==F1[4] && U[5]==F1[5]){

        printf("y= x^cos(x)\n\n");

        //regra do expoente

        printf("y= (e^(cos(x).ln(x)\n\n");

        // regra da cadeia f = e^u e u = cosxlnx

        printf("y= d/du (e^u) d/dx (cos(x).ln(x))\n\n");

        printf("d/du(e^u) = e^u e d/dx (cos(x).ln(x)) = -sin(x).ln(x) + cos(x)/x\n\n ");

        printf("y= e^u(-sin(x).ln(x)+(cos(x)/x))\n\n");

        //voltando u

        printf("y'= e^cos(x).ln(x)[-sin(x).ln(x) + (cos(x)/x)\n\n");

        //voltando na regra do expoente

        printf("y'= x^cos(x)[-sin(x)ln(x) + (cos(x)/x)\n\n");

        }else{

        printf("Opcao invalida\n");

        }



        if(U[0]==F2[0] && U[1]==F2[1] && U[2]==F2[2] && U[3]==F2[3] && U[4]==F2[4] && U[5]==F2[5]){

        printf("y= x^tg(x)\n\n");

        //regra do expoente

        printf("y= (e^(tg(x).ln(x)\n\n");

        // regra da cadeia f = e^u e u = cosxlnx

        printf("y= d/du (e^u) d/dx (tg(x).ln(x))\n\n");

        printf("d/du(e^u) = e^u e d/dx (tg(x).ln(x)) = sec^2.ln(x) + (tg(x)/x)\n\n ");

        printf("y= e^u[sec^2(x).ln(x) + (tg(x)/x)\n\n");

        // voltar u

        printf("y'= e^(tg(x).ln(x))[sec^2(x).ln(x) + (tg(x)/x)\n\n");

        printf("y'= x^tg(x)(sec^2(x).ln(x) + (tg(x)/x)\n\n");

        }

        break;

    case 2:

        printf("Digite o valor de U para a funcao x^(Ux^K)n\n");
        scanf("%lf",&U1);

        printf("Digite o valor de K para a funcao x^(Ux^K)\n\n");
        scanf("%lf",&U2);

        printf("\n\n");

        printf("y= x^(%.1lfx^%.1lf\n\n", U1, U2);

        // regra do expoente

        printf("d/dx (e^(%.1lfx^%.1lf . ln(x)\n\n",U1, U2);

        //regra da cadeia

        printf("d/du (e^u) d/dx (%.1lfx^%.1lf.ln(x))\n\n",U1,U2);

        Conta1 = U2 - 1;

        printf("d/du (e^u) = e^u e d/dx (%.1lfx^%.1lf.ln(x)) = %.1lf(%.1lfx^%.1lf . ln(x) + x^%.1lf\n\n",U1,U2,U1,U2,Conta1,Conta1);

        printf("e^u . [%.1lf(%.1lfx^%.1lf . ln(x) + x^%.1lf] \n\n", U1, U2, Conta1, Conta1);

        // voltando u

        printf("e^(%.1lfx^%.1lf . ln(x)) . [%.1lf(%.1lfx^%.1lf . ln(x) + x^%.1lf] \n\n",U1, U2, U1, U2, Conta1, Conta1);

        // voltando no expoente

        printf("%.1lfx^(%.1lfx^%.1lf) [ %.1lfx^%.1lf . ln(x) + x^%.1lf\n\n",U1,U1,U2,U2,Conta1,Conta1);

    }





}


int main(){

    printf("Seja Bem Vindo !!\n");

    printf("Escolha seu tipo de derivada\n\n");

    Menu();

    scanf("%d",&EscolhaDerivada);
    setbuf(stdin,NULL);

    switch(EscolhaDerivada){

    case 1:
        Poli1();

    break;

    case 2:
        Poli2();

    break;

    case 3:
        Poli3();

    break;

    case 4:
         Poli4();

    break;

    case 5:
         Poli5();

    break;

    case 6:
        Poli6();

    break;

    case 7:
         Poli7();

    break;

    case 8:
        Poli8();

    break;

    case 9:
        Poli9();

    break;

    case 10:
         Poli10();

    break;

    case 11:
         LNU();

    break;

    case 12:
         UN();

    break;

    case 13:
         UV();

    break;

    case 14:
         UV2();

    break;

    case 15:
         EU();

    break;

    case 16:
         SINU();

    break;

    case 17:
         COSU();

    break;

    case 18:
         TGU();

    break;

    case 19:
         SECU();

    break;

    case 20:
         COSSECU();

    break;

    case 21:
         COTGU();

    break;

    case 22:
         UV3();

    break;









}


}
