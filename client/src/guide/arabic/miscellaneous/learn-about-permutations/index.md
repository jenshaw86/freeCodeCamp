---
title: Learn About Permutations
localeTitle: تعرف على التباديل
---
_التقليب_ هو مصطلح رياضي لعدد من الطرق يمكن تجميع مجموعة من الكائنات في مجموعة. إنه يشبه مصطلح رياضي آخر ، _تركيبة_ ، باستثناء اختلاف رئيسي واحد: مع التباديل ، فإن ترتيب itmes في المجموعة يحدث فرقًا.

على سبيل المثال ، لنفترض أنك كنت تسحب الأرقام من قبعة وتعول المجموعات المختلفة من ثلاثة أرقام. في هذه الحالة ، سيكون كل من `[1,2,3]` و `[3,2,1]` مزيجًا من `1` و `2` و `3` ، وسيعتمد ذلك على مجموعة واحدة.

ومع ذلك ، إذا كنت تحسب تباينات للأرقام ، فسيتم حسابها كمثنتين مختلفتين لأن الأرقام الموجودة في كل مجموعة تكون بترتيب مختلف.

يمكن حساب التباديل بإحدى طريقتين ، اعتمادًا على ما إذا كان يتم السماح بالقيم المتكررة أم لا. لحساب عدد التباديل للكائنات `n` بدون تكرار ، يمكنك ببساطة حساب `n!` أو `n * (n-1) * (n-2) ... * 1` . وهذا أمر منطقي ، لأنه إذا اخترت رقمًا واحدًا من القبعة ولم تعيده قبل اختيار الرقم التالي ، فسيكون هناك عدد أقل للاختيار من بينها.

لحساب جزء فقط من إجمالي عدد التباديل (على سبيل المثال ، للعثور على عدد التباديل من ثلاثة أرقام من 1 إلى 10 بدون تكرار) ، تحتاج فقط إلى التكاثر لعدد الخيارات التي تقوم بها. في حالة الأرقام الثلاثة ، ستحتاج فقط إلى مضاعفة `10 * 9 * 8` . وبنفس الطريقة، **إذا** سمح يكرر (بمعنى، يمكنك وضع عدد مرة أخرى في قبعة بعد حصوله)، وكنت اضرب `10 * 10 * 10` .