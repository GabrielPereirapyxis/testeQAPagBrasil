describe('Form Submission', () => {
    it('teste funcional com dados validos', () => {
      cy.visit('www.formulariocontato.com');
  
      cy.get('#Name').type('NomeTeste');
  
      cy.get('#Email').type('email@teste.com');

      cy.get('#Company').type('Companhia teste');

      cy.get('#Website').type('www.companytest.com');

      cy.get('#Phone').type('(51)99999-9999');

      cy.get('#Inquiry').type('Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent malesuada dignissim ligula, eu ultrices ipsum eleifend a. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.u');
  
      cy.get('#btnSubmit').click();
  
      cy.contains('Sucesso');
    });
  });


  describe('Form Submission', () => {
    it('teste com caracteres especiais no campo name', () => {
      cy.visit('www.formulariocontato.com');
  
      cy.get('#Name').type('N0M& T&ST#@');
  
      cy.get('#Email').type('email@teste.com');

      cy.get('#Company').type('Companhia teste');

      cy.get('#Website').type('www.companytest.com');

      cy.get('#Phone').type('(51)99999-9999');

      cy.get('#Inquiry').type('Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent malesuada dignissim ligula, eu ultrices ipsum eleifend a. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.u');
  
      cy.get('#btnSubmit').click();
  
      cy.contains('Campo Name inválido.');
    });
  });

  describe('Form Submission', () => {
    it('teste sem preenchimento no campo phone', () => {
      cy.visit('www.formulariocontato.com');
  
      cy.get('#Name').type('Nome teste');
  
      cy.get('#Email').type('email@teste.com');

      cy.get('#Company').type('Companhia teste');

      cy.get('#Website').type('www.companytest.com');

      cy.get('#Inquiry').type('Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent malesuada dignissim ligula, eu ultrices ipsum eleifend a. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.u');
  
      cy.get('#btnSubmit').click();
  
      cy.contains('Campo Phone inválido.');
    });
  });
