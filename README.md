- š Hi, Iām @kdg9980
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

const { chromium } = require('playwright');
(async () => {
  const browser = await chromium.launch({
    headless: false
  });
  const context = await browser.newContext();

  await page.goto('http://lesha-spr.github.io/react-validation/');

  await page.locator('div:has-text("Firstname*")').nth(3).click();

  await page.getByPlaceholder('Firstname').click();

  await page.getByPlaceholder('Firstname').fill('ź¹ė² ģ“');

  await page.getByPlaceholder('Firstname').press('Tab');

  await page.getByPlaceholder('Lastname').fill('ė”ė³“');

  await page.getByPlaceholder('Lastname').press('Tab');

  await page.getByPlaceholder('Email').fill('bear@gmail.com');

  await page.getByRole('combobox', { name: 'City*' }).selectOption('3');

  await page.getByRole('textbox', { name: 'Password*' }).click();

  await page.getByRole('textbox', { name: 'Password*' }).fill('1004Qa%^&');

  await page.getByRole('textbox', { name: 'Password*' }).press('Tab');

  await page.getByPlaceholder('Confirm password').fill('1004Qa%^&');

  await page.locator('label:has-text("I accept policy*") div').click();

  await page.locator('form:has-text("RegistrationValidate allFirstname*Lastname*Email*City*Choose your cityLondonKyiv")').getByRole('button', { name: 'Submit' }).click();

  await page.locator('form:has-text("RegistrationValidate allFirstname*Lastname*Email*City*Choose your cityLondonKyiv")').getByRole('button', { name: 'Submit' }).click();

  await page.getByPlaceholder('Lastname').click();

  await page.locator('label:has-text("I accept policy*") div').click();

  await page.getByPlaceholder('Lastname').click();

  await page.getByPlaceholder('Lastname').fill('');

  await page.getByLabel('I accept policy*Required').check();

  await page.getByLabel('I accept policy*').uncheck();

  await page.getByLabel('I accept policy*Required').check();

  await page.getByPlaceholder('Lastname').click();

  await page.getByPlaceholder('Lastname').fill('ė”ė³“');

  await page.getByPlaceholder('Email').click();

  await page.getByText('I accept policy*').click();

  await page.locator('html').click();

  await page.getByPlaceholder('Email').dblclick();

  await page.getByText('RegistrationValidate allFirstname*Lastname*Email*City*Choose your cityLondonKyiv').click({
    clickCount: 3
  });

  await page.getByPlaceholder('Email').click();

  await page.getByPlaceholder('Email').fill('123#');

  await page.getByLabel('I accept policy*Required').check();

  await page.getByPlaceholder('username').click();

  await page.getByPlaceholder('username').fill('ź¹ė² ģ“ ');

  await page.getByPlaceholder('username').press('Tab');

  await page.locator('form:nth-child(2) > div:nth-child(2) > div:nth-child(2)').click();

  await page.getByPlaceholder('Leave your comment...').dblclick();

  await page.getByPlaceholder('Leave your comment...').fill('Hello ! how are you ? ģėķģøģ 1234');

  await page.locator('form:has-text("Leave a commentHello ! how are you ? ģėķģøģ 1234Submit")').getByRole('button', { name: 'Submit' }).click();

  await page.locator('form:has-text("Leave a commentHello ! how are you ? ģėķģøģ 1234Submit")').getByRole('button', { name: 'Submit' }).dblclick();

  await page.getByPlaceholder('username').click();

  await page.locator('form:has-text("Leave a commentHello ! how are you ? ģėķģøģ 1234Submit")').getByRole('button', { name: 'Submit' }).click();

  await page.getByPlaceholder('username').click();

  await page.getByPlaceholder('username').fill('');

  await page.getByPlaceholder('Leave your comment...').click();

  // ---------------------
  await context.close();
  await browser.close();
})();
