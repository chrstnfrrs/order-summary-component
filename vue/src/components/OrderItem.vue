<template>
  <div class="order-item">
    <div class="order-item-info">
      <figure>
        <img src="../assets/icon-music.svg" alt="" />
      </figure>
      <div class="order-item-info__col">
        <p class="order-item-info__name"><strong>Annual Plan</strong></p>
        <p class="order-item-info__price">$59.99/year</p>
      </div>
    </div>
    <p class="order-item-info__action">Change</p>
  </div>
</template>

<style lang="scss">
.order-item {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 2rem;
  background-color: var(--very-pale-blue);
  border-radius: 0.6875rem;
  width: 100%;
  padding: 1.5rem;
  &-info {
    display: flex;
    gap: 1rem;
    &__col {
      display: flex;
      flex-direction: column;
      gap: 0.375rem;
    }
    &__name {
      color: var(--dark-blue);
      font-weight: 900;
    }
    &__price {
      color: var(--desaturated-blue);
      font-weight: 500;
    }
    &__action {
      color: var(--bright-blue);
      font-size: 0.875rem;
      font-weight: 700;
      text-decoration: underline;
      cursor: pointer;
      text-underline-offset: 0.2rem;
    }
  }
}
</style>
